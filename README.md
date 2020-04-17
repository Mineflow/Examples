# MineflowExamples

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
