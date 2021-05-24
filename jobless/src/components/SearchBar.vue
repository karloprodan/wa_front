<template>
  <div id="SearchBar">
    <form>
    <!-- Pretraži poslove -->
      <input type="text" class="jobsName" placeholder="Pretraži ključne riječi..." />
    <!-- Pretraži djelatnosti -->
      <select class="jobsCategory">
          <option value="" style="font-weight: bold;">Sve djelatnosti</option>
          <option value="1" >Administrativna zanimanja</option>
          <option value="2">Arhitektura, dizajn i umjetnost</option>
          <option value="3">Državna služba i uprava</option>
          <option value="4">Ekonomija, računovodstvo i financije</option>
          <option value="5">Elektrotehnika</option>
          <option value="6">Farmacija, biotehnologija, kemija</option>
          <option value="7">Graditeljstvo i geodezija</option>
          <option value="8">Informatika i telekomunikacije</option>
          <option value="9">Instalacije, održavanje, popravak</option>
          <option value="10">Ljudski resursi</option>
          <option value="11">Management i upravljanje</option>
          <option value="12">Marketing, PR i mediji</option>
          <option value="13">Strojarstvo i brodogradnja</option>
          <option value="14">Neprofitne organizacije</option>
          <option value="15">Poljoprivreda</option>
          <option value="16">Prodaja (maloprodaja - veleprodaja)</option>
          <option value="17">Promet i transport</option>
          <option value="18">Skladištenje i logistika</option>
          <option value="19">Turizam i ugostiteljstvo</option>
          <option value="20">Zdravstvo, socijalni rad i skrb</option>
          <option value="21">Znanost i obrazovanje</option>
          <option value="22">Ostalo</option>

      </select>
    <!-- Pretraži županije -->
      <select class="jobsLocation">
          <option value="" style="font-weight: bold;">Sve županije</option>
          <option value="1">Bjelovarsko-bilogorska</option>
          <option value="2">Brodsko-posavska</option>
          <option value="3">Dubrovačko-neretvanska</option>
          <option value="4">Istarska</option>
          <option value="5">Karlovačka</option>
          <option value="6">Koprivničko-križevačka</option>
          <option value="7">Krapinsko-zagorska</option>
          <option value="8">Ličko-senjska</option>
          <option value="9">Međimurska</option>
          <option value="10">Osječko-baranjska</option>
          <option value="11">Požeško-slavonska</option>
          <option value="12">Primorsko-goranska</option>
          <option value="13">Sisačko-moslavačka</option>
          <option value="14">Splitsko-dalmatinska</option>
          <option value="15">Međimurska</option>  
          <option value="16">Varaždinska</option>
          <option value="17">Virovitičko-podravska</option>
          <option value="18">Vukovarsko-srijemska</option>
          <option value="19">Zadarska</option>
          <option value="20">Zagrebačka</option>
          <option value="21">Grad Zagreb</option>
      </select>

      <button type="button" class="botun">
        <span class="material-icons">
          search
        </span>
      </button>
    </form>
  </div>
</template>

<script>
export default {
  name: "SearchBar",
};
</script>

<style scoped>
#SearchBar {
  background-image: url("../assets/SearchBar_back.jpg");
  height: 133px;
  background-color: black;
  padding: 45px;
  display: flex;
  justify-content: center;
}

.jobsName {
    margin-right: 40px;
    padding-bottom: 2px;
    padding-left: 19px;
    width: 270px;
    border-radius: 20px;
    border: 1px solid black;
    font-family:'Segoe UI';
    font-size: 18px;
}
.jobsName:focus {
  outline: none;
}

input[type="text"].jobsName::-webkit-input-placeholder {
  color: rgb(93, 95, 98);
  font-style: italic;
}

.jobsCategory {
    margin-right: 20px;
    padding-bottom: 2px;
    padding-left: 13px;
    border-radius: 20px;
    border: 1px solid black;
    font-family:'Segoe UI';
    font-size: 18px;
    color: rgb(93, 95, 98);
}
.jobsCategory:focus {
  outline: none;
}

.jobsLocation {
    margin-right: 20px;
    padding-bottom: 2px;
    padding-left: 13px;
    border-radius: 20px;
    border: 1px solid black;
    font-family:'Segoe UI';
    font-size: 18px;
    color: rgb(93, 95, 98);
}
.jobsLocation:focus {
  outline: none;
}

.botun {
    background-color: #3DBC91;
    margin-left: 20px;
    border-radius: 20px;
    padding-left: 35px;
    padding-right: 35px;
    border: 1px solid black;
}

.material-icons {
    padding-top: 4px;
    font-size: 30px;
    font-weight: bold;
}

form {
    display: flex;
    justify-content: space-around;
}

</style>
