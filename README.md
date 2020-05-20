# MineflowExamples

# How To Use
jsonファイルをmineflow/importsフォルダに入れて`/mineflow`コマンドで読みこんでください  
Put the json file in the mineflow/imports folder and import it with `/mineflow` command  

## checkId
`/id` コマンドで手に持っているアイテムのidを表示する  
Send ID of the item in player's hand with the command `/id`.  

## TouchBlockInfo
触ったブロックの情報をtip欄に送る  
Send info about the block you touched to the tip field.  

## clank
`/clank`コマンドでお金を1000消費してガチャを引く  
Draw a lottery with the command "/clank".  
#### config: clank.yml
```
cost: <price>
items:
- id: <item id>
  count: <item count>
language: <jpn or eng>
```

## mobAI
殴ったエンティティが追いかけてくる(ジャンプはしません)  
The entity you attacked will track you down.  

## BlockPlaceCoolDown
[checkCoolDown](#checkCoolDown)の使用例  
Example for [checkCoolDown](#checkCoolDown)  

# functions
## checkCoolDown
指定した時間以内に呼び出すとfalseをそれ以外はtrueを返す  
使用方法:  
1. `スクリプト > ほかのレシピを呼び出す`で<name>に`aieuo/function/checkCoolDown`を、<args>に秒数を入力  
2. `スクリプト > もし...」`を追加する  
3. `もし`の条件に`スクリプト > 文字列を比較する`を追加して`{result}`と`true`が等しいか調べる  

使用例: [BlockPlaceCoolDown](#BlockPlaceCoolDown)  
Returns false if it is executed within the specified interval or less, and true otherwise.  
How to use:  
1. Enter `aieuo/function/checkCoolDown` in <name> and seconds in <args> of `Script > Call Other Recipes`  
2. Add the action `Script > if`  
3. Add `script > compare strings` to the condition and check if `{result}` is equal to `true`  

Examples: [BlockPlaceCoolDown](#BlockPlaceCoolDown)  
