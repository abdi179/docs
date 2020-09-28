---
title: 自動リンクされた参照と URL
intro: URL、Issue、プルリクエスト、コミットへの参照は、自動的に短縮されてリンクに変換されます。
redirect_from:
  - /articles/autolinked-references-and-urls
versions:
  free-pro-team: '*'
  enterprise-server: '*'
---

### URL

{{ site.data.variables.product.product_name }}は自動的に標準的な URL からリンクを生成します。

`https://github.com にアクセスしてください。`

![変換された自動リンク URL](/assets/images/help/writing/url-autolink-rendered.png)

リンクの生成に関する詳しい情報については[基本的な書き方とフォーマットの構文](/articles/basic-writing-and-formatting-syntax/#links)を参照してください。

### Issue およびプルリクエスト

{{ site.data.variables.product.product_name }} 上の会話の中では、Issue やプルリクエストへの参照は自動的に短縮リンクに変換されます。 詳細は「[{{ site.data.variables.product.prodname_dotcom }} 上の会話について](/articles/about-conversations-on-github)」を参照してください。

{% note %}

**メモ:** 自動リンクされた参照は、ウィキやリポジトリ中のファイルでは生成されません。

{% endnote %}

| 参照タイプ                                         | RAW 参照                                         | 短縮リンク                                                                  |
| --------------------------------------------- | ---------------------------------------------- | ---------------------------------------------------------------------- |
| Issue またはプルリクエストの URL                         | https://github.com/jlord/sheetsee.js/issues/26 | [#26](https://github.com/jlord/sheetsee.js/issues/26)                  |
| `#` および Issue またはプルリクエスト番号                    | #26                                            | [#26](https://github.com/jlord/sheetsee.js/issues/26)                  |
| `GH` および Issue またはプルリクエスト番号                   | GH-26                                          | [GH-26](https://github.com/jlord/sheetsee.js/issues/26)                |
| `ユーザ名/リポジトリ#` および Issue またはプルリクエスト番号          | jlord/sheetsee.js#26                           | [jlord/sheetsee.js#26](https://github.com/jlord/sheetsee.js/issues/26) |
| `Organization 名/リポジトリ#`および Issue またはプルリクエスト番号 | github/linguist#4039                           | [github/linguist#4039](https://github.com/github/linguist/pull/4039)   |

### コミット SHA

コミットの SHA ハッシュへの参照は、{{ site.data.variables.product.product_name }}上のコミットへの短縮リンクに自動的に変換されます。

| 参照タイプ          | RAW 参照                                                                               | 短縮リンク                                                                                                             |
| -------------- | ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------- |
| コミット URL       | https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e | [a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e)                   |
| SHA            | a5c3785ed8d6a35868bc169f07e40e889087fd2e                                             | [a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e)                   |
| ユーザ@SHA        | jlord@a5c3785ed8d6a35868bc169f07e40e889087fd2e                                       | [jlord@a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e)             |
| ユーザ名/リポジトリ@SHA | User/Repository@SHA: jlord/sheetsee.js@a5c3785ed8d6a35868bc169f07e40e889087fd2e      | [jlord/sheetsee.js@a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e) |

{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.18" %}
### 外部リソースへのカスタム自動リンク

{{ site.data.reusables.repositories.autolink-references }}

{% endif %}

### 参考リンク

- [基本的な書き方とフォーマットの構文](/articles/basic-writing-and-formatting-syntax)