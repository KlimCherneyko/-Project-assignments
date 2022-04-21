<template>
  <div class="app-footer">
    <div class="subscribe">
      <div class="sub">SUBSCRIBE</div>
      <input type="text" placeholder="enter your email">
      <div class="knopka-border"><button class="knopka">SUBMIT</button></div>
    </div>
    <div class="copyright">
      <div class="copyright-3">
        <span>© COPYRIGHT</span><span >{{ (new Date()).getFullYear() }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppFooter'

}
</script>

<style lang="scss" scoped>
.app-footer {
  .subscribe {
    height: 337px;
    background: #817070;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .sub{
    font-weight: 500;
    font-size: 36px;
    line-height: 53px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #FFFFFF;
    padding-top: 60px;
  }

  input {
  width: 300px;
  height: 55px;
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  font-weight: 300;
  font-size: 20px;
  line-height: 30px;
  text-align: center;
  color: #FFFFFF;
  border: 3px solid #FFFFFF;
  box-sizing: border-box;
  background: #817070;

    &::placeholder {
      color:#FFFFFF
    } 

  &:focus {
    outline: 0px;
    }
  }

  .knopka-border{
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;

    .knopka{
      width: 129px;
      height: 55px;
      background: #FFFFFF;
      border: 3px solid #FFFFFF;
      box-sizing: border-box;
      font-family: 'Oswald';  
      font-weight: 500;
      font-size: 20px;
      line-height: 30px;
      color: #817070;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 28px;
    }
  }



  .copyright {
    height: 72px;
    background: #E5E5E5;
    display: grid;

    .copyright-3 {
      margin-left: 35px;
      display: grid;
      justify-self: center;
      align-self: center;
      grid-template-columns: 1fr 1fr;
    }
  }
}
</style>