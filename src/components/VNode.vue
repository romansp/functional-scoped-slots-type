<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  render(h) {
    const children = this.$scopedSlots.default && this.$scopedSlots.default({});
    return h('div', children);
  },
});
</script>
