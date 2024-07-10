# 1. 製作遊戲背景
1. 打開小畫家->點擊油漆桶選黑色並在白色處點一下->對黑色背景點右鍵，選擇"調整大小"，點選像素並調整成600 * 800->另存新檔成.png檔(檔名我使用background.png)  
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/04944e01-db16-4a66-8e8c-cfd089e8089f)  
2. 打開Unity->打開background.png檔案所在位置，並將background拖曳至視窗下方的Assets處
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/7aac174b-d0ca-446b-862e-5a30ee8a84a9)
3. 把在Assets處的background拖曳到視窗上方Scene處
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/ad0e738c-eef6-4bad-b30f-ff42475584dd)
4. 點選視窗左方Hierarchy處的background物件，之後可看到視窗右方出現background的Inspector->將Inspector中Transform底下的Position其X、Y、Z都改成0讓在Scene的background置中    
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/f526025f-54d7-44ef-a1c5-0022975b8647)  
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/bf134ba4-d18d-4c7d-9c00-193260f36e13)  
5. 點選Inspector中Additional Settings底下的Sorting Layer右邊方塊，之後點選"Add Sorting Layer"  
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/1018cc05-041e-477f-a423-8a1494fbd0ee)  
6. 按下Sorting Layer底下 + 的圖案->新增Layer(Layer名稱我使用background)   
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/1f726d97-0264-4790-a7b4-dd8d69643d19)
7. 點擊視窗左方Hierarchy的background物件->點擊左方Inspector中Additional Settings底下的Sorting Layer右邊方塊，之後點選"background"
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/f0859c38-b926-4ea3-ad6e-2c8b7e50de62)

# 2. 製作飛機
1. 原作者自己畫了一台飛機，我自己是網路上隨便找一張圖片當作飛機用，將飛機照片像素調整成 50 * 50  
2. 將飛機拖曳至Assets->從Assets處把飛機拖曳至Scene->將飛機Position調整為 X:0、Y:-3、Z:0，讓飛機位置在background中下  
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/e6864276-918b-4b5e-a512-58548183b51d) ![image](https://github.com/unshun0120/space_shooter/assets/79517348/dd827415-0dcb-4442-9aaa-36049579be18)
3. 給予飛機碰重的屬性讓他會被敵人碰到->點擊Inspector最底下"Add Component"->選Physics 2D->選Box Collider 2D->選完後可看到碰種外框(綠色的那個)  
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/ee49770e-e56f-4eff-9986-b8d9b43426a5)  
4. 點擊Inspector中Box Collider 2D->將Size中的Y設為0.45讓判定不要太嚴格，設完後可以看到碰撞外框的大小有改變
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/d295a3a5-00ac-4c23-b90d-c4fe2487fede)  
5. 將飛機加入rigidbody的性質使其可以移動->點擊Inspector最底下"Add Component"->選Physics 2D->選Rigidbody 2D  
   將Rigidbody 2D下的Gravity Scale設為0(因為不需要重力)->點開下面的Constraints並勾選Freeze Rotation的Z(因為飛機不用旋轉)
   ![image](https://github.com/unshun0120/space_shooter/assets/79517348/a3b4fdf3-b65c-40ed-b732-04bb06b92e30)











