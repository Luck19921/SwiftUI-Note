# SwiftUI-Note
This is my note of learning SwiftUI
## About Text()
### 1.strikethrough() or strikethrough(_ active: Bool, color: Color? = nil)
> 將文字加上刪節線, 如果color = nil, 刪節線的顏色將會以系統預設為主
### 2.underline() or underline(_ active: Bool, color: Color? = nil) 
> 在文字底部加上底線, 顏色的部分同上述
### 3.kerning(_ kerning: CGFloat)
> 使該段文字中每一個字母或字元的間隔距離等同於CGFloat長度
### 4.tracking(_ tracking: CGFloat)
> 功能展現上貌似與上述kerning相同, 被用於設定字母或字元間的間隔距離
### 5.baselineOffset(_ baselineOffset: CGFloat)
> 將該段文字的位置稍微往上提升, 換句話說就是對文字的基礎位置做變更


## About Stack()
### VStack, HStack or ZStack
> x, y維度垂直, 水平與z維度完全蓋上主體
