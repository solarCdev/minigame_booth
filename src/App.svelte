<script>
  import logo from "./assets/logo.png";
  import card from "./assets/card.jpg";
  import dice from "./assets/dice.jpg";
  import casino from "./assets/casino.jpg";
  import tsunami from "./assets/tsunami.jpg";
  import python from "./assets/python.jpg";
  import watermelon from "./assets/watermelon.jpg";
  console.log(logo);
  
  const contents = [
    {
      name: '주사위 게임 🎲',
      description: '수를 예측해서 홀/짝을 맞춰보자!',
      img: dice,
      link: 'https://solarcdev.github.io/sungbin-dice/%EC%B5%9C%EC%A2%85.HTML'
    },
    {
      name: '자연재해 서바이벌 🌋',
      description: '산성비, 번개, 스나미 등 여러 자연재해로부터 살아남기!',
      img: tsunami,
      link: 'https://scratch.mit.edu/projects/757540875'
    },
    {
      name: '수박 게임 🍉',
      description: '우리가 아는 수박게임을 웹사이트로!',
      img: watermelon,
      link: 'https://kairess.github.io/suika-game'
    },
    {
      name: '슬롯머신 🎰',
      description: '확률의 신에게 기도하는 게임!',
      img: casino,
      link: 'https://solarcdev.github.io/casino/casino.html'
    },
    {
      name: '파이썬 게임 🐍',
      description: '플레이하려면 저희에게 말해주세요!',
      img: python,
      link: '/'
    },
    {
      name: '카드 플리퍼 🃏',
      description: '적당히의 미학을 게임으로 느껴보자!',
      img: card,
      link: 'https://solarcdev.github.io/flipper/flipper.html'
    },
  ]
</script>

<main>
  <nav>
    <img src={logo} alt="logo" class="logo">
  </nav>
  <div class="banner">
    <div class="banner-wrap">
      <h1>
        semicolon <br>
        Minigames!
      </h1>
      <h2>
        2023 세미콜론 미니게임부 팀원들의 미니게임을 즐겨보세요! <br>
        동아리에 참여하고 싶다면 동아리장 (30403 권호준)에게 말해주세요!
      </h2>
    </div>
  </div>
  <div class="wrap">
    {#each contents as content}
      <a href={content.link} target="_blank">
        <div class="card">
          <img src={content.img} alt="img" class="content-img">
          <div class="des-wrap">
            <h3>{content.name}</h3>
            <p>{content.description}</p>
          </div>
        </div>
      </a>
    {/each}
  </div>
  <footer>
    <span><strong>Semicolon ⓒ 2024 minigames.</strong></span> <br> <br>
    <span>세미콜론 미니게임 부스에 방문해주셔서 감사합니다! 동아리에 참여하고 싶다면 동아리장 (30403 권호준)에게 말해주세요!</span>
  </footer>
</main>

<style>
</style>
