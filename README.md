# Tシャツカラーシミュレーター

Tシャツの色とデザインの色をブラウザ上で変更し、プレビュー・書き出しができるシンプルなWebツールです。

---

## 機能

* Tシャツカラー変更
* デザインカラー変更（黒PNG前提）
* デザインの位置・サイズ調整
* 表 / 裏 切り替え
* 高解像度PNG書き出し（例：3000px）

---

## ファイル構成

<pre class="overflow-visible! px-0!" data-start="251" data-end="321"><div class="relative w-full mt-4 mb-1"><div class=""><div class="relative"><div class="h-full min-h-0 min-w-0"><div class="h-full min-h-0 min-w-0"><div class="border border-token-border-light border-radius-3xl corner-superellipse/1.1 rounded-3xl"><div class="h-full w-full border-radius-3xl bg-token-bg-elevated-secondary corner-superellipse/1.1 overflow-clip rounded-3xl lxnfua_clipPathFallback"><div class="pointer-events-none absolute end-1.5 top-1 z-2 md:end-2 md:top-1"></div><div class="relative"><div class="pe-11 pt-3"><div class="relative z-0 flex max-w-full"><div id="code-block-viewer" dir="ltr" class="q9tKkq_viewer cm-editor z-10 light:cm-light dark:cm-light flex h-full w-full flex-col items-stretch ͼd ͼr"><div class="cm-scroller"><div class="cm-content q9tKkq_readonly"><span>project/</span><br/><span>├── index.html</span><br/><span>├── shirt-front.png</span><br/><span>└── shirt-back.png</span></div></div></div></div></div></div></div></div></div></div><div class=""><div class=""></div></div></div></div></div></pre>

---

## 使い方

1. デザインPNG（黒ベース・透過）をアップロード
3. 色や位置を調整
4. 「保存」で画像を書き出し

---

## 画像仕様

### デザイン画像

* 黒1色 + 透過PNG
* グラデーション可
* 白背景はNG（透過必須）

---

## 解像度について

* 画面表示：900px
* 書き出し：3000px（変更可能）

変更箇所：

<pre class="overflow-visible! px-0!" data-start="600" data-end="635"><div class="relative w-full mt-4 mb-1"><div class=""><div class="relative"><div class="h-full min-h-0 min-w-0"><div class="h-full min-h-0 min-w-0"><div class="border border-token-border-light border-radius-3xl corner-superellipse/1.1 rounded-3xl"><div class="h-full w-full border-radius-3xl bg-token-bg-elevated-secondary corner-superellipse/1.1 overflow-clip rounded-3xl lxnfua_clipPathFallback"><div class="pointer-events-none absolute inset-x-4 top-12 bottom-4"><div class="pointer-events-none sticky z-40 shrink-0 z-1!"><div class="sticky bg-token-border-light"></div></div></div><div class="relative"><div class=""><div class="relative z-0 flex max-w-full"><div id="code-block-viewer" dir="ltr" class="q9tKkq_viewer cm-editor z-10 light:cm-light dark:cm-light flex h-full w-full flex-col items-stretch ͼd ͼr"><div class="cm-scroller"><div class="cm-content q9tKkq_readonly"><span class="ͼg">const</span><span> </span><span class="ͼm">EXPORT_SIZE</span><span> </span><span class="ͼg">=</span><span> </span><span class="ͼj">3000</span><span>;</span></div></div></div></div></div></div></div></div></div></div><div class=""><div class=""></div></div></div></div></div></pre>

## 注意

* 元画像の解像度が低いと書き出しも粗くなります
* 大きすぎる画像はブラウザが重くなる可能性あり

黒PNG画像をCSS maskとして使い、任意の色でTシャツ上に表示するサンプルです。
