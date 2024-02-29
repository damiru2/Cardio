<template>
  <div class="head">
    <div class="promotion">
      <span>NEW</span>
      Новая интенсивная тренировка
    </div>
    <div class="lead">
      <div>
        <h1>Cardio<br />Exercise</h1>
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Rem quos
          minima corporis reprehenderit architecto. Quia ipsa eaque maiores cum
          delectus.
        </p>
        <div class="lead__buttons">
          <button>Начать</button>
          <button>Детальнее</button>
        </div>
      </div>
      <div>
        <img src="/img/lead.png" alt="Workout" />
        <div class="lead__info">
          <div class="lead__info__time">
            <span>38:14</span>
            ВРЕМЯ
          </div>
          <div class="lead__info__cl">
            <span>165</span>
            КАЛОРИИ
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
.head {
  margin-top: 70px;
  overflow: hidden;
  height: 800px;
}

.promotion {
  background: #191919;
  border-radius: 200px;
  padding: 10px 5px;
  color: #d1d1d1;
  width: 330px;

  span {
    background: #25ab75;
    border-radius: 200px;
    padding: 5px 10px;
    color: #fff;
    margin-right: 10px;
    font-weight: 600;
  }
}

.lead {
  margin-top: 20px;
  display: flex;
  position: relative;

  h1 {
    font-size: 12em;
    line-height: 170px;
  }

  p {
    color: #868686;
    width: 600px;
    margin: 20px 0;
  }

  .lead__buttons > button {
    background: #25ab75;
    padding: 20px;
    width: 160px;
    font-weight: 600;
    font-size: 1.02em;
    color: #fff;
    border: 0;
    cursor: pointer;
    border-radius: 10px;
    margin-top: 30px;
    transition: transform 500ms ease;

    &:last-of-type {
      background: #191919;
      margin-left: 35px;
    }

    &:hover {
      transform: translateY(-7px);
    }
  }

  > div:last-of-type {
    img {
      position: relative;
      bottom: 255px;
      right: 270px;
    }

    .lead__info {
      position: absolute;
      top: 0;
      right: 0;

      @mixin info-block {
        background: #191919;
        border-radius: 20px;
        padding: 20px 30px;
        width: 110px;
        font-size: 0.7em;
        margin-bottom: 25px;

        span {
          font-weight: 600;
          font-size: 3em;
          display: block;
        }
      }

      .lead__info__time {
        @include info-block;

        span {
          color: #ffe642;
        }
      }
      .lead__info__cl {
        @include info-block;

        span {
          color: #fb1351;
        }
      }
    }
  }
}
</style>
