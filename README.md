# SwiftUI-Note
  This is my note of learning SwiftUI
  
  ## About Stack()
### VStack、HStack、ZStack(三種Stack畫布)
  > H、V與Z分別代表水平、垂直與立體三維空間作為畫布底, 三種Stack被應用於實現不同佈局需求。此外, 可以在使用各類Stack時在後方的()內添加init, 實際使用方式如下：VStack(alignment: , spacing: CGFloat) , alignment代表著此Stack內的元件的對齊規則(.leading、.center、.trailing), 分別代表著對左靠齊、居中對齊與對右靠齊。
  
## About Text()
### init(verbatim content: String)
  > 實際範例：Text("This is my Text!")
### strikethrough() or strikethrough(_ active: Bool, color: Color? = nil)
  > 將文字加上刪節線, 如果color = nil, 刪節線的顏色將會以系統預設為主。
### underline() or underline(_ active: Bool, color: Color? = nil) 
  > 在文字底部加上底線, 顏色的部分同上述。
### kerning(_ kerning: CGFloat)
  > 使該段文字中每一個字母或字元的間隔距離等同於CGFloat長度。
### tracking(_ tracking: CGFloat)
  > 功能展現上貌似與上述kerning相同, 被用於設定字母或字元間的間隔距離。
### baselineOffset(_ baselineOffset: CGFloat)
  > 將該段文字的位置稍微往上提升, 換句話說就是對文字的基礎位置做變更。

## About Button()
### init(action: @escaping ()->Void, @ViewBuilder label: ()-> Label)
  > 在使用Button時, 最為最基本的初始化, 只需要在action部分填上你希望當此按鈕被Click時, 有什麼變數會被toggle、有什麼func()將會被執行；後方的label部分則是填入Text("Your button name"), 即可為你的Button顯示出文字作為辨別。請看以下實際範例：
                    <pre><code>Button(action: {
                        self.myButtonClick.toggle() //action區塊, 可以做任何你想做的事情func、改變變數狀態等
                    }, label: {
                        Text("我是按鈕A") //label區塊, 此處可以編輯該Button欲以什麼字元被顯示
                    })</code></pre>
