# gitの運用について
## 概要
git-flowをベースに以下の関係で行う
<table>
<tr>
<td> main </td>
<td> 本番環境 </td>
</tr>
<tr>
<td> release </td>
<td> ステージング環境 </td>
</tr>
</table>

- Issueでタスク分けを行った際の番号を使用しする  
```
git switch -c 1_add_function
git switch -c #1_add_function
```

## 流れ
- releaseからチェックアウトして機能開発を行い、releaseにプルリク  
- 場合によってはdevelopを入れて、developからreleaseへ
