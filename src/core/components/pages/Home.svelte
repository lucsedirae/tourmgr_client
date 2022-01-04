<script>
  import { str_welcome_msg } from '../../../config/lang/template.json';
  import { str_register } from '../../../config/lang/lang.json';

  import Button from '../layout/Button.svelte';
</script>

<div class="container">
  <div>
    <p class="text-center">{str_welcome_msg}</p>
  </div>

  <div class="break" />

  <div>
    <Button>{str_register}</Button>
  </div>
</div>
