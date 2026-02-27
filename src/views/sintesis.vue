<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-5 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo:
    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="En la gestión de cuentas de usuario se tienen en cuenta: 1. Tipos de herramientas de administración de BC: pgAdmin4, PhpMyAdmin, Heidi SQL y Adminer. 2. Sistema de permisos: Read, ReadWrite, DbAdmin, DBOwner, UserAdmin. 3. Lengiaje de control DCL a. Grand: crea permisos en el sistema. b. Revoke: elimina permisos en el sistema. 4. Gestión de seguridad: contraseña expirada por defecto, contraseña sin expiración y contraseña expirada en un tiempo. 5. Ejecución de Scripts: creación de usuario y eliminación de usuario. ")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
