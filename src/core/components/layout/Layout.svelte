<script>
  import {siteName} from '../../../config/site/siteconfig.json'

  let todaysDate = new Date(Date.now()).toLocaleString().split(',')[0];

</script>

<div>
  <h1 class="text-center brand">{siteName}</h1>
  <p class="text-center light">{todaysDate}</p>
  <div class="container">
    <slot></slot>
  </div>
</div>