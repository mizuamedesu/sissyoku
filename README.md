# 失職検証

ChatGPT o1のテスト

<img width="1159" alt="スクリーンショット 2024-12-06 11 34 06" src="https://github.com/user-attachments/assets/25a2123a-5ae5-4d4d-842d-04d839238f51">
<img width="1470" alt="スクリーンショット 2024-12-06 11 34 29" src="https://github.com/user-attachments/assets/3faa3c93-9437-4cf9-9d3c-70121ee3c3f9">


```
user:こんな感じのアニプレみたいなモダンでおしゃれでアニメチックなサイトを作ってください。単一のhtmlファイルでおねがいします。(アニプレのサイトを添付)
```

```
o1:<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>モダンでアニメチックなラインナップサイト</title>
<style>
  body {
    margin: 0;
    font-family: 'Noto Sans JP', sans-serif;
    background: #f9f7f5;
    color: #333;
  }

  header {
    display: flex;
    align-items: center;
    padding: 0.5rem 1.5rem;
    background: #fff;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 999;
  }
  header img.logo {
    height: 40px;
    margin-right: 2rem;
  }
  nav {
    display: flex;
    gap: 1rem;
    font-size: 0.9rem;
    font-weight: 500;
  }
  nav a {
    text-decoration: none;
    color: #333;
    position: relative;
    padding: 0.5rem;
  }
  nav a:hover::after {
    content: "";
    position: absolute;
    bottom: 0; left: 0; right: 0;
    height: 2px;
    background: #333;
  }

  .main-visual {
    width: 100%;
    height: 300px;
    background: url('https://picsum.photos/2000/600?grayscale&blur=2') center/cover no-repeat;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #fff;
    font-size: 2rem;
    font-weight: 700;
    letter-spacing: 0.05em;
  }

  .line-up-section {
    max-width: 1200px;
    margin: 0 auto;
    padding: 2rem 1rem;
    text-align: center;
  }

  .line-up-section h2 {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    letter-spacing: 0.05em;
    position: relative;
  }

  .line-up-section h2::after {
    content: "LINE UP";
    position: absolute;
    font-size: 4rem;
    color: rgba(0,0,0,0.05);
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    pointer-events: none;
  }

  .kana-filter {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.5rem;
    margin-bottom: 2rem;
  }

  .kana-filter button {
    border: none;
    background: #fff;
    padding: 0.5rem 1rem;
    border-radius: 20px;
    font-size: 0.9rem;
    cursor: pointer;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    transition: background 0.2s;
  }
  .kana-filter button:hover {
    background: #f0f0f0;
  }

  .line-up-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill,minmax(150px,1fr));
    gap: 1.5rem;
  }

  .card {
    background: #fff;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
    cursor: pointer;
  }

  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.15);
  }

  .card img {
    width: 100%;
    display: block;
    aspect-ratio: 3/4;
    object-fit: cover;
  }

  .card-info {
    padding: 0.5rem;
    text-align: left;
    font-size: 0.9rem;
  }
  .card-info h3 {
    margin: 0.5rem 0;
    font-size: 1rem;
    font-weight: 700;
  }
  .card-info p {
    margin: 0;
    color: #555;
    font-size: 0.8rem;
  }

  footer {
    margin-top: 3rem;
    background: #fff;
    padding: 1rem;
    text-align: center;
    font-size: 0.8rem;
    color: #777;
    border-top: 1px solid #eee;
  }

  @media (max-width: 600px) {
    nav {
      flex-wrap: wrap;
    }
    nav a {
      padding: 0.5rem 0;
    }
    .main-visual {
      font-size: 1.5rem;
    }
  }
</style>
</head>
<body>
<header>
  <img src="https://aniplex.co.jp/favicon.ico" alt="Logo" class="logo">
  <nav>
    <a href="#">アニメ</a>
    <a href="#">ゲーム</a>
    <a href="#">舞台</a>
    <a href="#">イベント</a>
    <a href="#">その他</a>
    <a href="#">会社案内</a>
    <a href="#">スペシャル</a>
    <a href="#">公式通販</a>
    <a href="#">公式SNS</a>
  </nav>
</header>

<div class="main-visual">
  あなたの心を揺さぶるアニメの世界へ
</div>

<section class="line-up-section">
  <h2>作品一覧</h2>
  <div class="kana-filter">
    <button>ア行</button>
    <button>カ行</button>
    <button>サ行</button>
    <button>タ行</button>
    <button>ナ行</button>
    <button>ハ行</button>
    <button>マ行</button>
    <button>ヤ行</button>
    <button>ラ行</button>
    <button>ワ行</button>
    <button>検索</button>
  </div>

  <h3 style="text-align:left;font-weight:700;font-size:1.2rem;margin-bottom:1.5rem;">最新作</h3>
  <div class="line-up-grid">
    <div class="card">
      <img src="https://picsum.photos/400/600?random=1" alt="title1">
      <div class="card-info">
        <h3>作品タイトル１</h3>
        <p>幻想的な世界観が広がる新感覚ファンタジー。</p>
      </div>
    </div>
    <div class="card">
      <img src="https://picsum.photos/400/600?random=2" alt="title2">
      <div class="card-info">
        <h3>作品タイトル２</h3>
        <p>熱き戦いと友情が織りなすアクション巨編。</p>
      </div>
    </div>
    <div class="card">
      <img src="https://picsum.photos/400/600?random=3" alt="title3">
      <div class="card-info">
        <h3>作品タイトル３</h3>
        <p>青春が輝く学園ストーリー。</p>
      </div>
    </div>
    <div class="card">
      <img src="https://picsum.photos/400/600?random=4" alt="title4">
      <div class="card-info">
        <h3>作品タイトル４</h3>
        <p>闇夜に響くミステリーの調べ。</p>
      </div>
    </div>
  </div>
</section>

<footer>
  © 2024 AnimeLine Inc. All Rights Reserved.
</footer>
</body>
</html>
```
