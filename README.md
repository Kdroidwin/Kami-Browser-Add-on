# Kami-Browser-Add-on

- ⭐️⭐️⭐️必須
- ⭐️⭐️超おすすめ
- ⭐️　 おすすめ（実用性が高い）

- `Proprietary`       
開発元が独占的に所有・管理しているソフトウェアや技術
ソースコードは公開されず、改変・再配布に制限がある。
プロプライエタリだから危険、オープンソースだから安全というわけではないです。

## ガイド
同系統の機能は可能な限り1つに集約してください（例：広告ブロックはuBlock Originのみ）。
機能が重複すると、競合・誤動作・検出回避失敗の原因になります。
代用できるものはuBOやユーザースクリプトなどで統合するのが理想です。

あくまでこのリスト全部入れるのではなく選んで使ってください。

多くの拡張機能は「すべてのサイトのデータを読み取り・変更する」権限を持ちます。
不要な拡張を多数入れることは、情報漏洩やセキュリティリスクの増加につながります。
導入前に権限、最終更新日、開発状況、ソースコード、開発者を必ず確認しましょう。
このリストは「全部入れるリスト」じゃなくて「辞書として使うリスト」として使ってください。

GreasyForkはほとんど審査なしということも覚えておくべきです。

## セキュリティ&プライバシー

- **uBlock Origin (uBO)** ⭐️⭐️⭐️
  コンテンツブロッカー。CPUとメモリーの負担が少なく、要素非表示や my ルールなどの機能もある。  
  おすすめカスタムフィルター: [GitHub - yokoffing/filterlists](https://github.com/yokoffing/filterlists)  
  ClearURLs より Actually Legitimate URL Shortener Tool を入れるほうが良い。  
  このアドオンを入れている場合、Privacy Badger や DuckDuckGo Privacy Essentials、AdGuard などはインストールしないこと。  
  YouTube フィルタ、Shorts 削除、TextForma v3、EmoGuard、Negative News Filter の一部機能なども代用できる。  
  Chrome: [uBlock Origin](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=ja&pli=1)  
  Firefox: [uBlock Origin](https://addons.mozilla.org/ja/firefox/addon/ublock-origin/)

- **Malwarebytes Browser Guard**  
  悪意あるサイトのブロック。トラッカー、広告、悪意のあるコンテンツをブロックしてプライバシーを保護する。  
  uBlock Origin や AdGuard と併用する際は干渉するため、Ads/Tracker をオフにすること。Current Website ではなく歯車アイコン側から設定すること。  
  セキュリティの知識が多少あるなら、このアドオンは不要で uBO だけで十分かもしれない。  
  Chrome: [Malwarebytes Browser Guard](https://chromewebstore.google.com/detail/malwarebytes-browser-guar/ihcjicgdanjaechkgeegckofjjedodee?hl=en)  
  Firefox: [Malwarebytes Browser Guard](https://addons.mozilla.org/ja/firefox/addon/malwarebytes/)

- **Canvas Blocker**  
  Canvas-Fingerprinting を防ぐために `<canvas>` を変更するための JS-API をブロックまたは偽装する。  
  ただしこの拡張機能ではそこまで役に立たないレベルであるため、about:config 調整の方が良い。
  Firefox には組み込みの指紋防止機能があり、`privacy.resistFingerprinting` を `true` に設定することで有効にできるが、一部サイトで不具合が起きたり、自動的にウィンドウサイズが丸められるので注意。  
  プライバシーを重視した Firefox フォークなどはデフォルトで `privacy.resistFingerprinting` が有効になっている場合がある。  
  Chrome: [Canvas Blocker](https://chromewebstore.google.com/detail/canvas-blocker-fingerprin/nomnklagbgmgghhjidfhnoelnjfndfpd?hl=ja)  
  Firefox: なし

- **bypass-all-shortlinks-debloated** ⭐️⭐️ 
  迷惑なリンク短縮サービスを自動的にスキップする。  
  更新が停止した FastForward の代替として最もおすすめできる。  
  debloated とあるようにフォーク元からいらないコードを取り除いている。  
  AdsBypasser よりもこちらがよいが、両方入れても多くの場合は大丈夫。ただし干渉する恐れがあるので非推奨。  
  [Codeberg](https://codeberg.org/Amm0ni4/bypass-all-shortlinks-debloated)

- **Affiliate Killer**  
  アフィリンク & Google リダイレクトリンク削除。  
  [GreasyFork](https://greasyfork.org/ja/scripts/456-affiliate-killer)

---

## YouTube

- **Youtube polymer engine fixes**  
  YouTube のホームページの広告枠やショート動画をなくしたり、動画の幅や提案や正確ないいねを表示する。  
  [GreasyFork](https://greasyfork.org/en/scripts/405614-youtube-polymer-engine-fixes)

- **Enhancer for YouTube**  `Proprietary` 
  PIP 機能、音量ブースト、コメントと動画同時閲覧などができる。クローズドソース。  
  Chrome: [Enhancer for YouTube](https://chrome.google.com/webstore/detail/enhancer-for-youtube/ponfpcnoihfmfllpaingbgckeeldkhle?hl=ja)  
  Firefox: [Enhancer for YouTube](https://addons.mozilla.org/ja/firefox/addon/enhancer-for-youtube/)

- **YouTube LiveChat Flusher／弾幕チャット**  
  YouTube の live 動画やアーカイブ動画にニコニコ風コメントを追加できる。  
  Flow youtube chat は他のアドオンと干渉することがある。  
  Chrome: [YouTube LiveChat Flusher／弾幕チャット](https://chromewebstore.google.com/detail/youtube-livechat-flusher%EF%BC%8F/kkjglcpgfpjlaloboikfcoofameeljbe?hl=ja)  
  Firefox: [YouTube LiveChat Flusher／弾幕チャット](https://addons.mozilla.org/ja/firefox/addon/youtube-livechat-flusher/)

- **Youtube Speed up**  
  再生速度二倍より早くする。  
  [GreasyFork](https://greasyfork.org/en/scripts/421610-youtube-speed-up)

- **SponserBlock**  ⭐️⭐️
  YouTuber 自身による動画内広告や動画内の不要部分をスキップする。  
  Chrome: [SponsorBlock](https://chrome.google.com/webstore/detail/sponsorblock-for-youtube/mnjggcdmjocbbbhaepdhchncahnbgone)  
  Firefox: [SponsorBlock](https://addons.mozilla.org/ja/firefox/addon/sponsorblock/)

- **Return YouTube Dislike (RYD)**  
  YouTube の低評価数を表示する（推定であって正確ではない）。  
  個人的には他の拡張機能との干渉の点から、ユーザースクリプト版を推奨する。  
  [公式](https://www.returnyoutubedislike.com/install)  
  フォーク: [GreasyFork](https://greasyfork.org/ja/scripts/544392-return-youtube-dislike-pc-only)

- **YouTubeコメント欄の名前を元に戻す**  
  コメントのユーザー名を従来のユーザー名の形式に戻します。  
  [GreasyFork](https://greasyfork.org/ja/scripts/460361-return-youtube-comment-username)

- **YouTube™ の複数選択**  `Proprietary` 
  YouTube の動画を複数選択することを可能にする。まとめてプレイリストに追加などが可能。クローズドソース。  
  Chrome: [YouTube™ の複数選択](https://chromewebstore.google.com/detail/youtube-%E3%81%AE%E8%A4%87%E6%95%B0%E9%81%B8%E6%8A%9E/gpgbiinpmelaihndlegbgfkmnpofgfei?hl=ja)  
  Firefox: [YouTube™ の複数選択](https://addons.mozilla.org/ja/firefox/addon/multiselect-for-youtube/)

- **YouTube shorts block**  
  ショート動画を普通の動画にする。  
  Shorts 動画を見たくないだけなら uBO でよい。  
  Chrome: [YouTube shorts block](https://chrome.google.com/webstore/detail/youtube-shorts-block/jiaopdjbehhjgokpphdfgmapkobbnmjp?hl=ja)  
  Firefox: [YouTube shorts block](https://addons.mozilla.org/ja/firefox/addon/youtube-shorts-block/)

- **PocketTube**  `Proprietary` 
  YouTube のチャンネル グループ分け。クローズドソース。  
  Chrome: [PocketTube](https://chrome.google.com/webstore/detail/pockettube-youtube-subscr/kdmnjgijlmjgmimahnillepgcgeemffb?hl=ja)  
  Firefox: [PocketTube](https://addons.mozilla.org/ja/firefox/addon/youtube-subscription-groups/)

- **YouTube Premium Logo**  
  名前通り YouTube の左上のロゴを premium にするだけ。  
  [GreasyFork](https://greasyfork.org/en/scripts/445197-youtube-premium-logo)

- **Simple YouTube Age Restriction Bypass**  
  年齢認証を行わずに、YouTube で年齢制限のある動画を視聴。  
  [GreasyFork](https://greasyfork.org/en/scripts/423851-simple-youtube-age-restriction-bypass)

- **Tabview Youtube**  ⭐️
  動画の右側にコメントや動画の情報を表示。  
  [GreasyFork](https://greasyfork.org/en/scripts/428651-tabview-youtube)

- **DeArrow**  
  SponserBlock のように有志によって YouTube でより良いタイトルとサムネイルを実現。  
  [公式](https://dearrow.ajay.app)

- **Filmot Title Restorer**  
  プレイリストの中にある、削除済みの動画のタイトルを調べられる。Internet Archive にあるかどうかも確認可能。  
  [GreasyFork](https://greasyfork.org/ja/scripts/430202-filmot-title-restorer)

  Firefox なら動画をダブルクリックするだけでスクリーンショット（スナップショット）が可能。  
  特定のチャンネルを非表示にするアドオンを入れなくとも uBo でできる。  
  `Full title` にするのも uBO でできる。  
  youtube row fixer なども uBO で代用可能。  
  YouTube 拡張は競合が起きやすいため注意したい。

---

## 動画 音楽

- **Picture-in-Picture Extension (by Google)**  `Proprietary` 
  PIP 対応させる。クローズドソース。Firefox の場合はアドオンなしで可能。  
  Chrome: [Picture-in-Picture Extension (by Google)](https://chromewebstore.google.com/detail/picture-in-picture-extens/hkgfoiooedgoejojocmhlaklaeopbecg)  
  Firefox: 標準対応

- **AniSkip**  
  動画の OP スキップ。  
  [GreasyFork](https://greasyfork.org/en/scripts/457460-aniskip)

- **Streaming enhanced Netflix Disney Prime Video**  
  イントロとクレジットと広告をスキップするのはもちろん、再生速度コントロールなど様々な機能を追加。Crunchyroll や HBO Max にも対応。  
  [GitHub](https://github.com/Dreamlinerm/Netflix-Prime-Auto-Skip)

- **AbemaTV, ニコニコ風コメントスクロール**  
  AbemaTV にニコニコ風コメントスクロールを追加。  
  [Web Archive](https://web.archive.org/web/20240518204812/https://greasyfork.org/en/scripts/19235-abematv-%E3%83%8B%E3%82%B3%E3%83%8B%E3%82%B3%E9%A2%A8%E3%82%B3%E3%83%A1%E3%83%B3%E3%83%88%E3%82%B9%E3%82%AF%E3%83%AD%E3%83%BC%E3%83%AB)

- **コメント増量**  
  ニコニコ動画のコメントの表示量を増やす。  
  Chrome: [コメント増量](https://chromewebstore.google.com/detail/%E3%82%B3%E3%83%A1%E3%83%B3%E3%83%88%E5%A2%97%E9%87%8F/eeanibgekifamcnnieknbhjcoocnpipe?hl=ja)  
  Firefox: [コメント増量](https://addons.mozilla.org/ja/firefox/addon/%E3%82%B3%E3%83%A1%E3%83%B3%E3%83%88%E5%A2%97%E9%87%8F/)

- **Volume Control [Boost volume]**  
  音量を通常上限より大きくできる。  
  [GitHub](https://github.com/Chaython/volumecontrol)  
  Firefox: [Volume Control [Boost volume]](https://addons.mozilla.org/ja/firefox/addon/volume-control-boost-volume/)

- **SoundFixer**  
  タブごとに音量を調整できる。Chrome の方は非公式フォーク。  
  Chrome: [SoundFixer](https://chromewebstore.google.com/detail/soundfixer/mbhbddecpoendcifccfckjkigbinefkg)  
  Firefox: [SoundFixer](https://addons.mozilla.org/ja/firefox/addon/soundfixer/)

  ちなみに動画ダウンロードできるアドオンより yt-dlp を使うことを推奨。

---

## Twitter

- **Control Panel for Twitter**  ⭐️⭐️
  Twitter UI カスタマイズ、X アイコン変更、ForYou タブ削除。  
  Chrome: [Control Panel for Twitter](https://chromewebstore.google.com/detail/control-panel-for-twitter/kpmjjdhbcfebfjgdnpjagcndoelnidfj?hl=ja)  
  Firefox: [Control Panel for Twitter](https://addons.mozilla.org/ja/firefox/addon/control-panel-for-twitter/)

- **Twitter UI Customizer**  
  Twitter ツイート下ボタンメニュー UI 調整、サイドバー非表示など。  
  Chrome: [Twitter UI Customizer](https://chromewebstore.google.com/detail/twitter-ui-customizer/hpmhdmlhnppmmipefebkhkbpdcjiidmh?hl=ja)  
  Firefox: [Twitter UI Customizer](https://addons.mozilla.org/ja/firefox/addon/twitter-ui-customizer/)

- **TwitterX-One-Click-Blocker**  
  X/Twitter のツイートにワンクリックブロックボタンを追加。誤操作注意。  
  [GreasyFork](https://greasyfork.org/en/scripts/568421-twitterx-one-click-blocker)

- **Advanced Search for X（Twitter）🔍**  
  高度な検索、検索履歴、検索条件の保存。  
  [GreasyFork](https://greasyfork.org/ja/scripts/542403-advanced-search-for-x-twitter)

- **Clean-Spam-Link-Tweet(CSLT)**  
  ナイト系スパムツイートなどを非表示。  
  [GitHub](https://github.com/kawa-nobu/Clean-Spam-Link-Tweet)

- **Twitter(旧:𝕏)のインプレッション小遣い稼ぎ野郎どもをdisplay:none;するやつ**  
  インプレゾンビを非表示にする。  
  [GitHub](https://github.com/hi2ma-bu4/X_impression_hide)

  ちなみに Lightweight X (formerly Twitter) by menkuri は uBO に  
  `x.com##*:style(backdrop-filter: none !important;)`  
  を追加するだけで同じことができる。

---

## その他SNS

- **Pixiv Toolkit**  
  画像・小説ダウンローダー。epub 対応。  
  Chrome: [Pixiv Toolkit Next](https://chromewebstore.google.com/detail/pixiv-toolkit-next/ajlcnbbeidbackfknkgknjefhmbngdnj?hl=en)  
  Firefox: [Pixiv Toolkit](https://addons.mozilla.org/ja/firefox/addon/pixiv-toolkit/)

- **PixivPlus**  
  ID 検索機能。  
  [GreasyFork](https://greasyfork.org/ja/scripts/34153-pixiv-plus)

- **Pixiv Previewer**  
  Pixiv お気に入り数順などで並び替えや画像のプレビュー表示。  
  [GitHub](https://github.com/Ocrosoft/PixivPreviewer)

- **Reddit Enhancement Suite**  
  Reddit 機能追加。  
  [公式](https://redditenhancementsuite.com)

---

## 5chなどの掲示板サイト

- **5ch.io Direct Links**  
  5ch にある外部リンクのクッションページをなくし直リンに。  
  [GreasyFork](https://greasyfork.org/en/scripts/571229-5ch-io-direct-links)

- **SkipAntennaSite**  
  アンテナサイトをスキップ。  
  [GreasyFork](https://greasyfork.org/ja/scripts/16465-skipantennasite)

- **NicoDicBBSViewer**  
  ニコニコ大百科の NG 機能。  
  [GreasyFork](https://greasyfork.org/ja/scripts/2288-nicodicbbsviewer)

---

## 制限解除

- **Absolute Enable Right Click & Copy**  ⭐️
  文字選択禁止を強制的に解除するスクリプト。  
  同名の拡張機能があるが、権限を気にしないならこちらをインストールすることを強くおすすめする。  
  ただし、Android版Firefoxではバグがあるので Force Copy を代わりに使うことを強く勧める。  
  また、知識があるなら uBO スクリプトレットで代替できる。  
  [GreasyFork](https://greasyfork.org/ja/scripts/23772-absolute-enable-right-click-copy)

- **Convert Any links to Clickable Links**  
  URLやドメイン名（先頭の "h" が抜けている場合も含む）をクリック可能なリンクに変換する。  
  [記事](https://kdroidwin.hatenablog.com/entry/2025/02/23/124856)

- **Buster: Captcha Solver for Humans**  ⭐️
  reCAPTCHA（わたしはロボットではありません）を自動化できる（audio challenge のみ）。  
  Chrome: [Buster](https://chromewebstore.google.com/detail/buster-captcha-solver-for/mpbjkejclgfgadiemmefgebjfooflfhl)  
  Firefox: [レビュー](https://addons.mozilla.org/ja/firefox/addon/buster-captcha-solver/reviews/?score=2)

- **reCaptcha Autoclick**  
  reCaptcha のボタンを自動的にクリックする。  
  [GreasyFork](https://greasyfork.org/en/scripts/461650-recaptcha-autoclick)

- **hektCaptcha: hCaptcha Solver**  
  わたしはロボットではありませんのチェックを自動化。  
  Chrome: [hektCaptcha](https://chromewebstore.google.com/detail/hektcaptcha-hcaptcha-solv/bpfdbfnkjelhloljelooneehdalcmljb)  
  Firefox: [hektCaptcha](https://addons.mozilla.org/ja/firefox/addon/hektcaptcha/)

- **Bypass Paywall Clean**  ⭐️
  Paywall（毎日新聞などの有料記事）を回避。スマホで使うときは PC 版にすること。  
  Chrome: [bypass-paywalls-chrome-clean](https://gitflic.ru/project/magnolia1234/bypass-paywalls-chrome-clean)  
  Firefox: [bypass-paywalls-firefox-clean](https://gitflic.ru/project/magnolia1234/bypass-paywalls-firefox-clean)

- **Web Archives**  ⭐️
  ウェイバックマシン、インターネットアーカイブや検索エンジンのキャッシュなど様々なサイトのアーカイブを表示させる。  
  Chrome: [Web Archives](https://chromewebstore.google.com/detail/web-archives/hkligngkgcpcolhcnkgccglchdafcnao?hl=ja)  
  Firefox: [Web Archives](https://addons.mozilla.org/ja/firefox/addon/view-page-archive/)

- **SingleFile**  
  閲覧中のウェブページ全体を単一の html ファイルとしてダウンロード。  
  Chrome: [SingleFile](https://chrome.google.com/webstore/detail/singlefile/mpiodijhokgodhhofbcjdecpffjipkle)  
  Firefox: [SingleFile](https://addons.mozilla.org/ja/firefox/addon/single-file/)

- **「Show more」ボタンを自動で押す**  ⭐️
  「続きを読む」「記事全文を読む」を自動でクリック。  
  Shift + `;` で自動クリックする要素を設定できる。  
  [GreasyFork](https://greasyfork.org/en/scripts/415141-show-more-%E3%83%9C%E3%82%BF%E3%83%B3%E3%82%92%E8%87%AA%E5%8B%95%E3%81%A7%E6%8A%BC%E3%81%99)

- **続きを読むリンククリック**  
  Yahoo!Japanニュースや gooニュースの「続きを読む」「記事全文を読む」を自動でクリック。  
  上ので Shift + `;` で十分なのでこれは不必要だが、モバイルではそれが難しいので必要。  
  [GreasyFork](https://greasyfork.org/en/scripts/419030-%E7%B6%9A%E3%81%8D%E3%82%92%E8%AA%AD%E3%82%80%E3%83%AA%E3%83%B3%E3%82%AF%E3%82%AF%E3%83%AA%E3%83%83%E3%82%AF)

---

## 検索エンジン

- **uBlacklist**  ⭐️⭐️
  任意のサイトを検索サイトに表示させない。  
  購読リストからルールセットを購読することができる。  
  自分が作成した[ルール](https://github.com/Kdroidwin/uB-filter-by-kdroidwin)もあるので是非。  
  Chrome: [uBlacklist](https://chromewebstore.google.com/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe?hl=ja)  
  Firefox: [uBlacklist](https://addons.mozilla.org/ja/firefox/addon/ublacklist/)

- **Google Tool Button Clicker**  
  Google検索のツールボタン自動クリック。  
  [GreasyFork](https://greasyfork.org/ja/scripts/31255-google-tools-button-clicker)

- **AlternativeSearchengines2**  
  Google検索時に Bing、Yandex、DuckDuckGo の検索を追加。  
  Kiwi Browser では使えないかも。  
  [GreasyFork](https://greasyfork.org/en/scripts/8928-alternative-search-engines-2)

- **SearXNGにGemini AIの回答を表示 ✨**  
  APIキー必須。  
  [GitHub](https://github.com/koyasi777/searxng-gemini-answer-injector)

- **Search Result Previews**  
  検索結果に webページのプレビューを表示する。  
  Chrome: [Search Result Previews](https://chromewebstore.google.com/detail/search-result-previews/cedcejfiniojnlhlfhcppenochinijfo)  
  Firefox: [Search Result Previews](https://addons.mozilla.org/en-US/firefox/addon/search_result_previews/)

- **SearXNG-Remove-Specified-Languages-for-Japanese**  
  all と日本語と英語と中国語以外の選択を削除。  
  [GitHub](https://github.com/Kdroidwin/SearXNG-Remove-Specified-Languages-for-Japanese)

- **Reddit on Google Search**  
  Google検索時に Reddit だけにフィルターをかける。  
  [GreasyFork](https://greasyfork.org/en/scripts/462356-reddit-on-google-search)

- **Reddit on SearXNG Search**  
  SearXNG で Reddit だけに絞り込んだ検索を行う。  
  [GitHub](https://github.com/Kdroidwin/Reddit-on-SearXNG-Search)

- **ContextSearch web-ext**  
  テキストを選択して、コンテキストメニューやタイル式のポップアップから、インストール済みの検索エンジンで検索できる。  
  新しい検索エンジンを追加したり、ファビコンやクエリ文字列を編集することも可能。高度にカスタマイズ可能。  
  Chrome: [ContextSearch web-ext](https://chromewebstore.google.com/detail/contextsearch-web-ext/ddippghibegbgpjcaaijbacfhjjeafjh)  
  Firefox: [ContextSearch web-ext](https://addons.mozilla.org/ja/firefox/addon/contextsearch-web-ext/)

---

## 機能追加

- **Violentmonkey**  ⭐️⭐️⭐️
  自分でスクリプト（簡単に言うと JS ファイル単体で作る拡張機能みたいなもの）を作ったり、他の人が作ったスクリプトをインストールできる。  
  Tampermonkey と同様に使える。  
  こちらはオープンソースで最新。  
  [公式](https://violentmonkey.github.io/get-it/)

  MutationObserver 乱用した DOM 監視をするユーザースクリプトは重くなるので、入れすぎには注意したい。

- **ブックマークサイドバー**  
  ブックマークサイドバーが使える。  
  Chrome: [ブックマークサイドバー](https://chromewebstore.google.com/detail/%E3%83%96%E3%83%83%E3%82%AF%E3%83%9E%E3%83%BC%E3%82%AF%E3%82%B5%E3%82%A4%E3%83%89%E3%83%90%E3%83%BC/jdbnofccmhefkmjbkkdkfiicjkgofkdh?hl=ja)  
  Firefox: [Firefox のサイドバーを使用して、ブックマークや履歴、ソーシャル機能にアクセスする](https://support.mozilla.org/ja/kb/use-firefox-sidebar-access-bookmarks-history-synced)

- **Textarea Cache**  
  自動的に入力フォームに入力したテキストを保存してくれる。  
  [GitHub](https://github.com/wildskyf/TextareaCache?tab=readme-ov-file)

- **FoxyProxy**  
  プロキシ管理。  
  Chrome: [FoxyProxy](https://chromewebstore.google.com/detail/foxyproxy/gcknhkkoolaabfmlnjonogaaifnjlfnp?hl=ja)  
  Firefox: [FoxyProxy Standard](https://addons.mozilla.org/ja/firefox/addon/foxyproxy-standard/)

- **Link Gopher**  
  ページ内に存在するリンクを別タブに書き出してくれる。  
  Chrome: [Link Gopher](https://chromewebstore.google.com/detail/link-gopher/bpjdkodgnbfalgghnbeggfbfjpcfamkf?hl=ja)  
  Firefox: [Link Gopher](https://addons.mozilla.org/ja/firefox/addon/link-gopher/)

- **Pagetual**  ⭐️⭐️
  AutoPagerize に比べ、SearXNG で uBlacklist を使っていたときなど、一番下の要素が隠ぺいされているときでも対応しやすい。  
  次のページを自動で読み込み、繋げてくれる。  
  Infy Scroll や uAutoPagerize などよりも良い。  
  [GreasyFork](https://greasyfork.org/en/scripts/438684-pagetual)

- **User-Agent Switcher and Manager**  ⭐️
  ユーザーエージェント変更。PC でもモバイル表示にしたり、「お使いのブラウザには対応していません」を回避できる。ホワイトリスト方式も可能。  
  Chrome: [User-Agent Switcher and Manager](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg/related?hl=ja)  
  Firefox: [User-Agent Switcher and Manager](https://addons.mozilla.org/ja/firefox/addon/user-agent-string-switcher/)

- **W.A.R. Links Checker Premium**  
  ファイルアップローダーサイトのリンクを自動的にチェック。  
  [GreasyFork](https://greasyfork.org/en/scripts/2024-war-links-checker-premium)

- **GitHub Directory Download / Download GitHub Directory**  
  GitHub のディレクトリをまとめてダウンロードできる。  
  Chrome: [GitHub Directory Download](https://chromewebstore.google.com/detail/github-directory-download/bdclldlpokfdgjffkneljdknpgomgicc?hl=en)  
  Firefox: [Download GitHub Directory](https://addons.mozilla.org/ja/firefox/addon/download-github-directory/)

- **Cookie-Editor**  
  Cookie 編集。一般人は非推奨。  
  Chrome: [Cookie-Editor](https://chromewebstore.google.com/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm?hl=ja)  
  Firefox: [Cookie-Editor](https://addons.mozilla.org/ja/firefox/addon/cookie-editor/)

- **simpleGesture / Gesturefy**  
  マウスジェスチャー。  
  Chrome: [simpleGestures](https://chromewebstore.google.com/detail/simplegestures/flfminafiamnggnldfpilnfnmbgmiegn)  
  Firefox: [Gesturefy](https://addons.mozilla.org/ja/firefox/addon/gesturefy/)

- **auto-clip**  
  選択したテキストをクリップボードに自動的にコピーする。  
  [GitHub](https://github.com/DoumanAsh/auto-clip)

- **Refresh Web Page Regularly**  
  ページの自動更新。  
  [GitHub](https://github.com/Volta0719/refresh-web-chrome)  
  Firefox: [Refresh Web Page Regularly](https://addons.mozilla.org/en-US/firefox/addon/refresh-web-page-regularly/)

- **Death To _blank**  
  勝手に新規タブで開いてしまうリンクを同じタブでページ遷移できるようにする。  
  Firefox では `about:config` で `browser.link.open_newwindow -> 1` にすれば OK。  
  ちなみに `browser.link.open_newwindow -> 3`、`browser.link.open_newwindow.restriction -> 0` にすると、新規ウィンドウで開こうとするリンクも新しいタブで開くようになる。  
  Chrome: [Death To _blank](https://chromewebstore.google.com/detail/death-to-blank/gneobebnilffgkejpfhlgkmpkipgbcno)  
  Firefox: なし

- **TWP - Translate Web Pages**  
  ウェブページを翻訳。  
  [GitHub](https://github.com/FilipePS/Traduzir-paginas-web)  
  Firefox: [TWP - Translate Web Pages](https://addons.mozilla.org/ja/firefox/addon/traduzir-paginas-web/)

- **Bitwarden** ⭐️  
  パスワードマネージャー。  
  Chrome: [Bitwarden パスワードマネージャー](https://chromewebstore.google.com/detail/bitwarden-%E3%83%91%E3%82%B9%E3%83%AF%E3%83%BC%E3%83%89%E3%83%9E%E3%83%8D%E3%83%BC%E3%82%B8%E3%83%A3%E3%83%BC/nngceckbapebfimnlniiiahkandclblb?hl=ja)  
  Firefox: [Bitwarden - 無料パスワードマネージャー](https://addons.mozilla.org/ja/firefox/addon/bitwarden-password-manager/)

  自分でホストしたい場合は Bitwarden でもよいが、[KeePassXC ブラウザ](https://addons.mozilla.org/ja/firefox/addon/keepassxc-browser/) でもよい。

## AI

- **ChatGPT Ctrl+Enter で送信**  
  ChatGPT や Claude のウェブページで Ctrl+Enter または Cmd+Enter を押してメッセージを送信する。Enter キーだけを押すと改行される。  
  [GreasyFork](https://greasyfork.org/ja/scripts/500314-chatgpt-ctrl-enter-%E4%BB%A5%E7%99%BA%E9%80%81)

- **KeepChatGPT**  
  ChatGPT にいくつかの機能を追加。ChatGPT のエラー解決にも使える。  
  [GreasyFork](https://greasyfork.org/en/scripts/462804-keepchatgpt)

- **Video to Article Next**  
  YouTube 動画を要約（画像付き）。  
  [GitHub](https://github.com/k0range/video2article-next)

- **Geminiによる要約と翻訳**  
  Web サイトを翻訳して要約、もしくは要約だけ。  
  Chrome: [Geminiによる要約と翻訳](https://chromewebstore.google.com/detail/gemini%E3%81%AB%E3%82%88%E3%82%8B%E8%A6%81%E7%B4%84%E3%81%A8%E7%BF%BB%E8%A8%B3/hmdcbbbdmfapkpdaganadiihfmdnpngi?hl=ja)  
  Firefox: [Geminiによる要約と翻訳](https://addons.mozilla.org/ja/firefox/addon/summarize-translate-gemini/)

## デザイン

- **Dark Reader**  ⭐️⭐️
  ほぼ全てのサイトをダークモード表示に。  
  Chrome: [Dark Reader](https://chromewebstore.google.com/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh?hl=ja)  
  Firefox: [Dark Reader](https://addons.mozilla.org/ja/firefox/addon/darkreader/)

- **Stylus**  
  CSS の知識があれば web ページの表示を変えられる。  
  `userstyles.world` から好きなユーザースタイルをインストール可能。  
  Chrome: [Stylus](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne?hl=ja)  
  Firefox: [Stylus](https://addons.mozilla.org/ja/firefox/addon/styl-us/)

- **Easy Speed Dial**  
  スピードダイアル（ホーム画面）を自由に調整。  
  [GitHub](https://github.com/lucaseverett/easy-speed-dial)

## ショッピング

- **Amazon.co.jpの商品ページに各種リンク追加**  
  商品ページに固定URL、サクラチェッカー、Keepa などのリンクを追加する。  
  [GreasyFork](https://greasyfork.org/ja/scripts/440936-amazon-co-jp%E3%81%AE%E5%95%86%E5%93%81%E3%83%9A%E3%83%BC%E3%82%B8%E3%81%AB%E5%90%84%E7%A8%AE%E3%83%AA%E3%83%B3%E3%82%AF%E8%BF%BD%E5%8A%A0)

- **Keepa – Amazon 価格トラッカー**  `Proprietary` 
  Amazon で売られている商品の値段の変化をグラフで表示。クローズドソース。  
  Chrome: [Keepa](https://chromewebstore.google.com/detail/keepa-amazon-price-tracke/neebplgakaahbhdphmkckjjcegoiijjo?hl=ja)  
  Firefox: [Keepa](https://addons.mozilla.org/ja/firefox/addon/keepa/)

- **Amazon CPU Tamer Pro**  
  Amazon の CPU 使用率の削減。  
  [GreasyFork](https://greasyfork.org/ja/scripts/533590-amazon-cpu-tamer-pro)

- **Condler**  
  Amazon 検索結果の左側サイドバーに、価格、人気度、レビューが良い順などの並び替え、Amazon 公式出品のみに絞り込むボタンを追加する。  
  [GitHub](https://github.com/nunawa/condler?tab=readme-ov-file)

- **AugmentedSteam**  
  Steam のカスタマイズ。所持しているゲームを緑色で表示したり、発売から現在までで最も安かった販売価格を表示。  
  [GitHub](https://github.com/IsThereAnyDeal/AugmentedSteam)

## 画像＆ダウンロード関連

- **DownThemAll!**  
  画像などを一括ダウンロード。  
  Chrome: [DownThemAll!](https://chromewebstore.google.com/detail/downthemall/nljkibfhlpcnanjgbnlnbjecgicbjkge?hl=en)  
  Firefox: [DownThemAll!](https://addons.mozilla.org/ja/firefox/addon/downthemall/)

- **Double-click Image Downloader**  
  画像をダブルクリックで保存する拡張機能。  
  Chrome: [Double-click Image Downloader](https://chrome.google.com/webstore/detail/double-click-image-downlo/bkijmpolkanhdehnlnabfooghjdokakc)  
  Firefox: [Double-click Image Downloader](https://addons.mozilla.org/en-US/firefox/addon/double-click-image-download/)  
  代替: [GreasyFork](https://greasyfork.org/en/scripts/469594-double-click-image-downloader)

- **Picviewer CE+**  
  写真を自動的にポップアップ・拡大・縮小・回転・バッチ保存できるオンラインの強力な画像表示ツール。  
  [GreasyFork](https://greasyfork.org/en/scripts/24204-picviewer-ce)

- **Search by Image**  
  画像検索。  
  Chrome: [Search by Image](https://chrome.google.com/webstore/detail/search-by-image/cnojnbdhbhnkbcieeekonklommdnndci)  
  Firefox: [Search by Image](https://addons.mozilla.org/firefox/addon/search_by_image/)

- **Imagus Reborn**  
  マウスカーソルを画像の上に置くことで、その画像を拡大表示。  
  Chrome: [Imagus Reborn](https://chromewebstore.google.com/detail/imagus-reborn/fcjmgeodgobggcppooncdagfkogfffdm)  
  Firefox: [Imagus Reborn](https://addons.mozilla.org/en-US/firefox/addon/imagus-reborn/)

## Firefox

- **Progressive Web Apps for Firefox**  
  Firefox で PWA。Floorp は不要。  
  [Firefox Add-ons](https://addons.mozilla.org/ja/firefox/addon/pwas-for-firefox/)

- **Search on Google Lens**  
  Firefox で Google Lens。ダウンロードした xpi ファイルを 7-Zip などで解凍すると Vivaldi などでも使える。  
  [Firefox Add-ons](https://addons.mozilla.org/ja/firefox/addon/search-on-google-lens/)  
  [GitHub](https://github.com/typeling1578/Search-on-Google-Lens)

- **fx_cast**  
  Firefox で Chromecast を有効に。  
  [公式](https://hensm.github.io/fx_cast/)

- **Tab Mix Plus**  
  タブ関係の設定をカスタマイズする。タブをクリックしたときの設定やマウスオーバーでタブを開くなど。  
  [GitHub](https://github.com/onemen/TabMixPlus)

  ちなみに最後のタブを閉じても Firefox が終了しないようにするには `browser.tabs.closeWindowWithLastTab` を `false` にすればよい。  
  ブックマークを現在のタブではなく新しいタブに開きたいなら `browser.tabs.loadBookmarksInTabs` を `true` にする。

- **Tree Style Tab**  
  Floorp 10 であったようなツリー型タブを実現。  
  [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/)

- **CRX Installer**  
  一部の Chrome 拡張機能を Firefox にインストールできる。セキュリティ的にはあまり推奨はできない。  
  [Firefox Add-ons](https://addons.mozilla.org/ja/firefox/addon/crxinstaller/)

- **DownExtZip**  
  Chrome ウェブストアや AMO（Firefox アドオン配布サイト）などからソースコードをダウンロード。  
  [Firefox Add-ons](https://addons.mozilla.org/ja/firefox/addon/downextzip/)

## モバイル向け

- **Simple Gesture for Android**  
  Android 向けジェスチャー。  
  [GitHub](https://github.com/utubo/firefox-simple_gesture)

- **MTDeck forked**  
  TweetDeck をスマホ UI に。  
  [GitHub](https://github.com/Kdroidwin/MTDeck_forked)

## テーマ

- **Black**  
  テーマ。  
  [Firefox Add-ons](https://addons.mozilla.org/ja/firefox/addon/black21/)
