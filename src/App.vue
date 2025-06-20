<script setup></script>

<template>
  <main>
    <img
      class="contens-img"
      src="./components/icons/サンベール1-4.png"
      alt=""
    />
    <img
      class="contens-img"
      src="./components/icons/サンベール2-2.png"
      alt=""
    />
    <img
      class="contens-img"
      src="./components/icons/サンベール3-2.png"
      alt=""
    />

    <div class="btn-inner1">
      <a href="#">
        <img src="./components/icons/サンベール-ボタン.png" alt="ボタン" />
      </a>
    </div>

    <div class="btn-inner2">
      <a href="#">
        <img src="./components/icons/サンベール-ボタン.png" alt="ボタン" />
      </a>
    </div>
    <!-- <form>
      姓：<input type="text" placeholder="山田" /> 名：<input
        type="text"
        placeholder="花子"
      />
      セイ：<input type="text" placeholder="ヤマダ" /> メイ：<input
        type="text"
        placeholder="ハナコ"
      />
      <select name="blood">
        <option value="女性">女性</option>
        <option value="男性">男性</option>
      </select>
      〒<input type="text" placeholder="0123456" />
      <select name="pref">
        <option value="">選択してください</option>
        <option value="北海道">北海道</option>
        <option value="青森県">青森県</option>
        <option value="岩手県">岩手県</option>
        <option value="宮城県">宮城県</option>
        <option value="秋田県">秋田県</option>
        <option value="山形県">山形県</option>
        <option value="福島県">福島県</option>
        <option value="茨城県">茨城県</option>
        <option value="栃木県">栃木県</option>
        <option value="群馬県">群馬県</option>
        <option value="埼玉県">埼玉県</option>
        <option value="千葉県">千葉県</option>
        <option value="東京都" selected>東京都</option>
        <option value="神奈川県">神奈川県</option>
        <option value="新潟県">新潟県</option>
        <option value="富山県">富山県</option>
        <option value="石川県">石川県</option>
        <option value="福井県">福井県</option>
        <option value="山梨県">山梨県</option>
        <option value="長野県">長野県</option>
        <option value="岐阜県">岐阜県</option>
        <option value="静岡県">静岡県</option>
        <option value="愛知県">愛知県</option>
        <option value="三重県">三重県</option>
        <option value="滋賀県">滋賀県</option>
        <option value="京都府">京都府</option>
        <option value="大阪府">大阪府</option>
        <option value="兵庫県">兵庫県</option>
        <option value="奈良県">奈良県</option>
        <option value="和歌山県">和歌山県</option>
        <option value="鳥取県">鳥取県</option>
        <option value="島根県">島根県</option>
        <option value="岡山県">岡山県</option>
        <option value="広島県">広島県</option>
        <option value="山口県">山口県</option>
        <option value="徳島県">徳島県</option>
        <option value="香川県">香川県</option>
        <option value="愛媛県">愛媛県</option>
        <option value="高知県">高知県</option>
        <option value="福岡県">福岡県</option>
        <option value="佐賀県">佐賀県</option>
        <option value="長崎県">長崎県</option>
        <option value="熊本県">熊本県</option>
        <option value="大分県">大分県</option>
        <option value="宮崎県">宮崎県</option>
        <option value="鹿児島県">鹿児島県</option>
        <option value="沖縄県">沖縄県</option>
      </select>
      <input type="text" placeholder="〇〇市△△区□町" />

      <input type="text" placeholder="1-1○○マンション101号" />
      <input type="text" placeholder="例）00000000000" />
      <input type="text" placeholder="support@kancha.jp" />

      <input type="date" name="calendar" max="9999-12-31">
      <input type="checkbox" name="check" id="check" />
      <label for="japan"
        >未成年者の場合、親権者の同意を得ております。（成人の方はチェック不要です）</label
      >

      <button type="submit" name="button" value="送信"></button>
    </form> -->
  </main>
</template>

<style scoped>
a:hover {
  background-color: rgba(10, 10, 100, 0);
}

header {
  line-height: 1.5;
}

.temp {
  display: inline-block;
}

main {
  background-color: #ffff;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  overflow: hidden;
  position: relative;
}

.btn-inner1 {
  position: absolute;
  top: 91.6%;

  /* background: #333333; */
  a {
    display: block;
    width: 32.291666vw;
    height: 7.375vw;

    img {
      width: 100%;
      height: auto;
      -webkit-transition: all 0.3s;
      transition: all 0.3s ease;
    }

    :hover {
      opacity: 0.7;
    }
  }
}

.btn-inner2 {
  position: fixed;
  top: 88%;

  /* background: #333333; */
  a {
    display: block;
    width: 32.291666vw;
    height: 7.375vw;

    img {
      width: 100%;
      height: auto;
      transition: all 0.6s ease;
      -webkit-transition: all 0.6s;
    }

    :hover {
      transform: scale(1.1, 1.1);
    }
  }
}

.contens-img {
  width: 100%;
  height: auto;
}

/* PCのブレイクポイント */
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .btn-inner1,
  .btn-inner2 {
    a {
      min-width: 650px;
      min-height: 140px;
    }
  }

  .contens-img {
    width: 100%;
    height: auto;
  }
}

/* タブレットのブレイクポイント */
@media screen and (min-width: 768px) and (max-width: 1024px) {
  .btn-inner1,
  .btn-inner2 {
    a {
      min-width: 600px;
      min-height: 130px;
    }
  }

  .contens-img {
    width: 100%;
    height: auto;
  }
}

/* スマホのブレイクポイント */
@media screen and (max-width: 480px) {
  .btn-inner1,
  .btn-inner2 {
    a {
      width: 80vw;
      height: 17.5vw;
      min-width: 250px;
      min-height: 55px;
    }
  }

  .contens-img {
    width: 100%;
    height: auto;
  }
}
</style>
