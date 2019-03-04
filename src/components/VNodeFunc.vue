<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  functional: true,
  render(h, ctx) {
    const children = ctx.scopedSlots.default && ctx.scopedSlots.default({});
    return children || h();
  },
});
</script>
