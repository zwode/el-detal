<template>
  <div class="d-flex mt-2">
    <div class="feedback-block">
      <div class="d-flex justify-content-between feedback-rate">
        <div class="feedback-date "> 22 февраля 2024 </div>
          <div class="rate align-self-center">
            <input type="radio" id="star5" name="rate" value="5" />
            <label for="star5" title="text">5 stars</label>
            <input type="radio" id="star4" name="rate" value="4" />
            <label for="star4" title="text">4 stars</label>
            <input type="radio" id="star3" name="rate" value="3" />
            <label for="star3" title="text">3 stars</label>
            <input type="radio" id="star2" name="rate" value="2" />
            <label for="star2" title="text">2 stars</label>
            <input type="radio" id="star1" name="rate" value="1" />
            <label for="star1" title="text">1 star</label>
          </div>
      </div>
      <div class="feedback-title">
        Алина Владимировна
      </div>
      <div class="feedback-text">
        Плиты от компании 21 век оказались надежным материалом для изготовления моей гардероба. Они не только просты в обработке, но и имеют высокую стойкость к царапинам и истиранию. К тому же, они доступнее по цене, среди конкурентов
      </div>
    </div>
    <div class="feedback-block">
      <div class="d-flex justify-content-between feedback-rate">
        <div class="feedback-date "> 22 февраля 2024 </div>
        <div class="rate">
          <input type="radio" id="star5" name="rate" value="5" />
          <label for="star5" title="text">5 stars</label>
          <input type="radio" id="star4" name="rate" value="4" />
          <label for="star4" title="text">4 stars</label>
          <input type="radio" id="star3" name="rate" value="3" />
          <label for="star3" title="text">3 stars</label>
          <input type="radio" id="star2" name="rate" value="2" />
          <label for="star2" title="text">2 stars</label>
          <input type="radio" id="star1" name="rate" value="1" />
          <label for="star1" title="text">1 star</label>
        </div>
      </div>
      <div class="feedback-title">
        Алина Владимировна
      </div>
      <div class="feedback-text">
        Плиты от компании 21 век оказались надежным материалом для изготовления моей гардероба. Они не только просты в обработке, но и имеют высокую стойкость к царапинам и истиранию. К тому же, они доступнее по цене, среди конкурентов
      </div>
    </div>
    <div class="feedback-block">
      <div class="d-flex justify-content-between feedback-rate">
        <div class="feedback-date "> 22 февраля 2024 </div>
        <div class="rate">
          <input type="radio" id="star5" name="rate" value="5" />
          <label for="star5" title="text">5 stars</label>
          <input type="radio" id="star4" name="rate" value="4" />
          <label for="star4" title="text">4 stars</label>
          <input type="radio" id="star3" name="rate" value="3" />
          <label for="star3" title="text">3 stars</label>
          <input type="radio" id="star2" name="rate" value="2" />
          <label for="star2" title="text">2 stars</label>
          <input type="radio" id="star1" name="rate" value="1" />
          <label for="star1" title="text">1 star</label>
        </div>
      </div>
      <div class="feedback-title">
        Алина Владимировна
      </div>
      <div class="feedback-text">
        Плиты от компании 21 век оказались надежным материалом для изготовления моей гардероба. Они не только просты в обработке, но и имеют высокую стойкость к царапинам и истиранию. К тому же, они доступнее по цене, среди конкурентов
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.feedback-block {
  padding: 20px 30px;
  width: 33.4%;
  background: #fff;
  border: 0.1px solid #777;
  transition: all 0.2s ease-in-out;
}

.feedback-date {
  padding-top: 6px;
}

.feedback-block:hover {
  transform: scale(1.05);
  transition: all 0.2s ease-in-out;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
}

.feedback-text {

}

.feedback-title {
  margin-bottom: 10px;
  font-size: 20px;
  font-weight: bold;
}
.rate {
  float: left;
  height: 46px;
  padding: 0 10px;
}
.rate:not(:checked) > input {
  position:absolute;
  top:-9999px;
}
.rate:not(:checked) > label {
  float:right;
  width:1em;
  overflow:hidden;
  white-space:nowrap;
  cursor:pointer;
  font-size:22px;
  color:#ccc;
}
.rate:not(:checked) > label:before {
  content: '★ ';
}
.rate > input:checked ~ label {
  color: #ffc700;
}
.rate:not(:checked) > label:hover,
.rate:not(:checked) > label:hover ~ label {
  color: #deb217;
}
.rate > input:checked + label:hover,
.rate > input:checked + label:hover ~ label,
.rate > input:checked ~ label:hover,
.rate > input:checked ~ label:hover ~ label,
.rate > label:hover ~ input:checked ~ label {
  color: #c59b08;
}


</style>
