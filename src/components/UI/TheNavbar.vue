<template>
  <mdb-navbar color="stylish" dark>
<!--    <mdb-navbar-brand href="#">-->
<!--      Navbar-->
<!--    </mdb-navbar-brand>-->
    <mdb-navbar-toggler>
      <mdb-navbar-nav>
        <mdb-nav-item href="#" class="active"><router-link to="/">Home</router-link></mdb-nav-item>
        <mdb-nav-item href="#"><router-link to="/about">About</router-link></mdb-nav-item>
        <mdb-nav-item href="#"><router-link to="/future">Future</router-link></mdb-nav-item>
      </mdb-navbar-nav>

      <!-- Indicates a successful or positive action -->
<!--      <mdb-btn>Resume</mdb-btn>-->
      <mdb-btn color="elegant">Resume</mdb-btn>
    </mdb-navbar-toggler>
  </mdb-navbar>
</template>

<script>
import { mdbNavbar, mdbNavbarToggler, mdbNavbarNav, mdbNavItem, mdbBtn  } from 'mdbvue';
export default {
name: "TheNavbar",
  components: {
    mdbNavbar,
    // mdbNavbarBrand,
    mdbNavbarToggler,
    mdbNavbarNav,
    mdbNavItem,
    mdbBtn
  }
}
</script>

<style scoped>
.navbar {
  /*height: 6rem;*/
  /*background: transparent;*/
  /*position: sticky;*/
  /*display: flex;*/
  /*align-items: center;*/
  /*justify-content: center;*/
}
/*@media screen and (max-width: 800px){*/
/*  .navbar {*/
/*    height: 10rem;*/
/*  }*/
/*}*/
a {
  color: var(--clr-white);
  /*margin-right: 3rem;*/
  letter-spacing: var(--spacing);
  transition: var(--transition);
  font-size: 1rem;
  /*border: 1px solid var(--clr-white);*/
  /*border-radius: var(--radius);*/
  padding: 0.1rem 1rem;
}
a:hover{
  color: var(--clr-black);
  /*background-color: var(--clr-white);*/
}
.btn{
  color: var(--clr-white);
  background: transparent;
  border: 1px solid var(--clr-white);
  padding: 0.1rem 0.75rem;
  display: inline-block;
  text-transform: uppercase;
  letter-spacing: var(--spacing);
  /*border-radius: var(--radius);*/
  transition: var(--transition);
}
.btn:hover {
  background: var(--clr-white);
  color: var(--clr-black);
}

</style>