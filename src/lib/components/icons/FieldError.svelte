<script lang="ts">
  import type { SVGAttributes } from 'svelte/elements'

  type $$Props = SVGAttributes<SVGElement>
</script>

<svg role="img" viewBox="0 0 24 24" {...$$restProps}>
  <circle cx="12" cy="12" r="10"></circle>
  <line x1="12" x2="12" y1="8" y2="12"></line>
  <line x1="12" x2="12.01" y1="16" y2="16"></line>
</svg>
