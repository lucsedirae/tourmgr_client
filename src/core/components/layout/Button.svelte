<script>

</script>

<button class="btn" ><slot /></button>

<style>
  .btn {
    color: var(--tertiary-light);
    border: 0;
    border-radius: 8px;
    background-color: var(--primary);
    width: 100px;
    height: 40px;
    cursor: pointer;
  }

  .btn:hover {
    transform: scale(0.98);
    background-color: var(--primary-dark);
  }
</style>
