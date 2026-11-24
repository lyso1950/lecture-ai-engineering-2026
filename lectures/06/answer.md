# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前： search_materials
- STEP 2 の [tool call]： glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]： glossary_search_glossary({'query': 'MCP'})
- STEP 4 の [tool call]： aws_aws___search_documentation({'search_phrase': 'Amazon S3 バージョニング 概要'})、aws_aws___search_documentation({'search_phrase': 'What is S3 Versioning'})
- 気づき・疑問：外部で動くサーバー(aws)の場合、tool callは2回起こっている。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎
- やったこと：app/mcp_server.pyにおいてTODOの行の下にserver.tool()(tools.get_lecture_summary)を追加した
- 結果：エージェント側を変えずに、一覧にglossary_get_lecture_Summeryが増えた。
- 気づき・疑問：エージェントは起動するごとに、公開されているツールの一覧をサーバーに問い合わせるという。
