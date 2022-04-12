<template>
  <ul class="list-menu">
    <li>
      <!-- child category -->
      <a href="#" data-toggle="collapse" :data-target="'#'+'collapse-'+category.slug+category.id" aria-expanded="true" class="">
        <i v-if="hasChildren" class="icon-control fa fa-chevron-down"></i>
        <span :class="hasChildren ? 'font-weight-bold' : '' "  > {{category.title}} </span>
      </a>
      <div v-if="hasChildren" class="filter-content collapse show ml-2" :id="'collapse-'+category.slug+category.id" style="">
        <TreeCategoryFilterMenu
          v-for="chil in category.child"
          :key="chil.id"
          :category="chil"
        />
      </div>
      <!-- child category -->
    </li>
  </ul>
</template>

<script>
export default {
  name: "TreeCategoryFilterMenu",
  props: {
    category: {
      type: Object,
      required: true
    }
  },
  computed: {
    hasChildren() {
      const { child } = this.category
      return child && child.length > 0
    }
  },
}
</script>

<style>

</style>
