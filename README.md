# comp6721
counter four





## Test results (Double-Card-2nd-Version):

| # | command input  | configuration image | test result | comments |
| -:|------------------|:--------------------|:------------|:---------|
| #1|  dots <br> 0 1 A 2  | <img src="test_result_images/configuration-1-test-hanging-position.jpg" width="380">  | 测试通过 | 测试放置悬空的卡片 |
| #2|  dots <br> 0 1 A 1 <br> 0 1 B 2 | <img src="test_result_images/configuration-2-test-hanging-position.jpg" width="380">  | 测试通过  | 测试放置半悬空的卡片  |
| #3|  dots <br> 0 1 H 1 | <img src="test_result_images/configuration-3-test-out-of-board-x-position.jpg" width="380">  | 测试通过  | 测试卡片片段超出board x轴情况  |
| #4|  dots <br> 0 2 B 1 <br> 0 4 A 1 <br> 0 1 A 3 <br> 0 2 B 4 <br> 0 8 A 4 <br> 0 6 A 6 <br> 0 4 A 8 <br> 0 2 A 10 <br> 0 2 A 12 | <img src="test_result_images/configuration-4-test-out-of-board-y-position.jpg" width="380">  | 测试通过  | 测试卡片片段超出board y轴情况  |
| #5|  dots <br> 0 5 A 1 <br> 0 2 A 2 <br> 0 6 D 1 <br> 0 4 B 2 <br> 0 8 C 1 <br> 0 7 C 3 <br> 0 1 A 4 <br> 0 7 C 4 <br> 0 6 C 5 | <img src="test_result_images/configuration-5-player1-wins.jpg" width="380">  | Failed | 测试在player1放置0 6 C 5卡片后，player1和player2同时满足赢的状态下，判定player1赢 |
| #6|  dots <br> 0 1 B 1 <br> 0 2 D 1 <br> 0 2 E 1 <br> 0 1 D 3 <br> 0 2 F 1 | <img src="test_result_images/configuration-6-player1-wins.jpg" width="380">  | Failed  | 测试在player1回合落字后，判定player1赢的情况  |
| #7|  dots <br> 0 1 B 1 <br> 0 2 D 1 <br> 0 2 E 1 <br> 0 2 F 1 | <img src="test_result_images/configuration-7-player1-wins.jpg" width="380">  | Failed  | 测试在player2回合落字后，判定player1赢的情况  |
| #8|  dots <br> 0 1 A 1 <br> 0 1 C 1 <br> 0 3 F 1 <br> 0 8 E 1 <br> 0 4 H 1 <br> 0 3 A 2 <br> 0 4 G 2 <br> 0 1 C 2 <br> 0 2 H 3 <br> 0 4 A 3 <br> 0 6 B 3 <br> 0 3 C 3 <br> 0 2 G 4 <br> 0 4 A 5 <br> 0 2 C 4 <br> 0 6 D 4 <br> 0 2 B 5 <br> 0 3 A 7 <br> 0 5 A 8 <br> 0 1 A 9 <br> 0 2 H 5 <br> 0 6 F 2 <br> 0 8 E 3 <br> 0 2 G 6 <br> recycle moves start <br> A 9 B 9 2 F 4 | <img src="test_result_images/configuration-8-recycle-starts.jpg" width="380"> <br><br> (recycle moves start) <br><br> <img src="test_result_images/configuration-8-recycle-player1-wins.jpg" width="380"> <br> position: (A 9 B 9) -> (F 4) <br> rotation: 1->2 | 未测试 | player1 在recycle moves环节，移动卡片(A 9 B 9)至(F 4) 并且改变旋转1至2 <br> 在player1和player2同时满足赢的情况下，判定player1赢 | 
| #8|   |   |   |

in the configuration images:
> **Blue square** means the piece that player1 drops

> **Orange square** means the piece that player2 drops

> **Green square** means that the winning position

> **card with Grey shallow** means that the card that has been moved to another place in recycle moves
