<template>
  <div class="works container">
    <h1 class="mb-5">Works</h1>
    <ul id="worksList">
      <li v-for="item in items" v-bind:key="item.id" class="mb-5">
        <div class="img">
          <img :src="item.img" class="img-fluid mx-auto d-block" />
        <p class="my-5">{{ item.coment }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { id: 1, img: "https://picsum.photos/1110/700",
        coment: '大阪・淀屋橋にあるタルタルガ様のWebサイトをリニューアルさせていただきました。6年ぶりのリニューアルということもあり、レスポンシブ化以外にも英語、中国語のページを作成するなど大きくバージョンアップしています。プランニングからデザイン、写真・動画撮影まで担当させていただきました。' },
        { id: 2, img: "https://picsum.photos/1110/700",
        coment: '大阪・福島 メリヤス会館内にあるstudio Tao様のWebサイトを制作させていただきました。ヨガのクラスやフラワーアレンジメントのワークショップなどを行なわれている素敵なスタジオです。プランニングからデザイン、ロゴ制作、写真撮影まで担当させていただいています。' },
        { id: 3, img: "https://picsum.photos/1110/700",
        coment: 'LOGI Terminal様のWebサイトを制作させていただきました。物流専門職の養成や物流相談など、物流業務改善に関わる業務をされています。定期的に更新されるブログはとても面白いので、物流に興味のある方はぜひのぞいてみてください。プランニングからデザイン、コーディングまで担当させていただいています。' },
        { id: 4, img: "https://picsum.photos/1110/700",
        coment: '大阪でストーリー・記事制作をされているScreen様のWebサイトを制作させていただきました。ロゴのデザイン、プランニングからデザイン、コーディングまで担当させていただいています。' },
      ]
    };
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Mansalva|Noto+Serif+JP&display=swap");

* {
  font-family: "Mansalva", cursive;
  font-family: "Noto Serif JP", serif;
}

ul {
  list-style: none;
  padding: 0;
}
</style>