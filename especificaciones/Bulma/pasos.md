Una vez instalado el bulma, creamos una carpeta llamada scss en src

# En la carpeta scss crearmos un archivo llamado App.scss y colocamos:
@import '../../node_modules/bulma/bulma.sass';
@import './helpers/helpers';

# Luego en App.vue agregamos los style:
<style lang="scss">
  @import './scss/App.scss';
</style>