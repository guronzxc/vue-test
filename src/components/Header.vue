<script setup></script>

<template>
  <header>
    <div class="header__content">
      <div class="header__links">
        <a href="#">
          <img src="@/assets/img/location.svg" alt="geotag" />
          <span id="location">Красноярск</span>
        </a>
        <a href="#" id="shop">Магазины</a>
        <div class="dropdown">
          <a href="#" class="dropbtn">
            <span id="buyers">Покупателям</span>
            <img src="@/assets/img/arrow.svg" alt="arrow" />
          </a>
          <div class="dropdown-content">
            <a href="#">link1</a>
            <a href="#">link2</a>
            <a href="#">link3</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#" class="dropbtn">
            <span id="company">Компания</span>
            <img src="@/assets/img/arrow.svg" alt="arrow" />
          </a>
          <div class="dropdown-content">
            <a href="#">link1</a>
            <a href="#">link2</a>
            <a href="#">link3</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#" class="dropbtn">
            <span id="organizations">Организациям</span>
            <img src="@/assets/img/arrow.svg" alt="arrow" />
          </a>
          <div class="dropdown-content">
            <a href="#">link1</a>
            <a href="#">link2</a>
            <a href="#">link3</a>
          </div>
        </div>
        <a href="#" id="promo">Акции</a>
        <a href="#" id="article">Статьи</a>
        <a href="#" id="gifts">Подарочные карты</a>
      </div>
      <div class="header__phone">
        <a href="tel:88007750070w3020"
          ><span id="boldtel">8(800)775-00-70 доб.3020</span
          ><span id="ordertel"> (бесплатно по России)</span></a
        >
      </div>
    </div>

    <div class="headersubmenu">
      <div class="submenu">
        <a id="cenalom" href="#"
          ><img src="@/assets/img/cenalom.svg" alt="cenalom"
        /></a>
        <button href="#" id="btnmenu">
          <img src="@/assets/img/iconburgermenu.svg" />КАТАЛОГ
        </button>
        <div class="divsearch">
          <form class="search">
            <input
              class="searchinput"
              type="search"
              placeholder="Искать здесь..."
            />
            <button class="searchbtn" type="submit">
              <img src="@/assets/img/search.svg" alt="search" />
            </button>
          </form>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.search {
  position: relative;
  width: 300px;
}
.searchinput,
.searchbtn {
  border: none;
  outline: none;
  border-radius: 3px;
}
.searchinput {
  width: 100%;
  height: 42px;
  padding-left: 15px;
  border: 1px solid grey;
}
.searchbtn {
  height: 26px;
  width: 35px;
  position: absolute;
  top: 8px;
  right: 8px;
  background-color: white;
}

#btnmenu {
  background: #ffee00;
  align-items: center;
  display: flex;
  padding: 6px;
}

#cenalom {
  display: flex;
  margin-top: 6px;
}

.header__content {
  max-width: var(--widthApp);
  background: var(--bgGray);
  margin: 0 auto;
  padding: 0 8px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 44px;
}

.headersubmenu {
  max-width: var(--widthApp);
  margin: 0 auto;
  padding: 0 8px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 44px;
  background-color: white;
}

.header__links {
  display: flex;
  position: relative;
  align-items: center;
  gap: 12px;
}

.submenu {
  display: flex;
  position: relative;
  align-items: center;
  gap: 12px;
}

.header__links a {
  display: flex;
  align-items: center;
  gap: 4px;
}

.dropdown-content {
  display: none;
  position: absolute;
  background: var(--bgGray);
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown:hover .dropdown-content {
  display: block;
}

#boldtel {
  font-weight: bolder;
  font-size: 20px;
}

#ordertel {
  font-weight: 300;
}

/* .header__links a {
  margin-right: 12px;
}

.header__links a:last-child {
  margin: 0;
} */

.header__links a,
.header__phone a {
  color: white;
}
</style>
