<template>
  <div class="personal-description-grid">
    <div class="main">
      <n-card
      hoverable>
        <h1>Yinsheng Zhou</h1>
        <h2>(site still under construction)</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laudantium
          adipisci, aut culpa recusandae totam esse, quis itaque quaerat
          laboriosam ea eum dolor, minima magnam? Iusto similique nam id quia
          fugit?
        </p>
      </n-card>
    </div>

      <!--profile card-->
      <div class="profile profile-grid">
        <n-card title="Profile" :bodered="true" hoverable>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Impedit mollitia temporibus obcaecati sit adipisci ducimus iusto quam veniam! Illo provident possimus corrupti a ab, labore sit, eveniet veritatis officia odio minus iste rem. Rerum, eius magni. Odio voluptatem quis necessitatibus saepe tempore consequatur dolorum suscipit laborum recusandae pariatur impedit perferendis ex accusamus, omnis, delectus rerum fugiat dolore hic rem animi tempora reprehenderit. Tempora ratione quod quo, corrupti tempore odit maiores est ad aperiam veritatis officiis eveniet, accusantium aliquam non in dolores possimus? Provident assumenda, nesciunt nemo, voluptate accusamus adipisci a ratione quisquam atque consequatur similique error beatae ut, ad nisi!</p>
        </n-card>
      </div>
      <!--profile card-->

      </div>


</template>

<script>
import { NCard } from "naive-ui";

export default {
  components: {
    NCard,
  },
};
</script>

<style scoped>
/* .main {
  display: grid;

}
 */

.profile {

 margin-top:10px;
  text-transform: capitalize;
}



a {
  color: black;
}
a:link {
  text-decoration: none;
}

</style>
