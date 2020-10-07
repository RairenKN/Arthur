1.In CE: File - Open process. for DX9: ffxiv.exe, DX11: ffxiv_dx11.exe

CE에서 : 프로세스 열기 (DDX9: ffxiv.exe, DX11: ffxiv_dx11.exe)

2.In game: Zoom all the way out, make sure there are no obstructions

인게임에서 : 장애물 없이 끝까지 줌 아웃

3.In CE: On the right side, change Value Type to Float. Look for Value 20.0

CE에서 : 오른쪽창에서 Value Type을 Float로 변경, 값 20.0을 찾는다.

4.In game: Zoom all the way in without going to first person

인게임에서 : 1인칭 사용하지 않고 끝까지 줌 인

5.In CE: Change Value to 1.5, hit enter or click "Next Scan"

CE에서 : 값을 1.5로 변경, 엔터 or 클릭으로 "Next Scan"

6.Repeat steps 2-5 until you see the value of interest in the window on the left. You should see the value changing as you change zoom in game.

2-5단계를 반복하며 줌을 인게임에서 바꾸기. 왼쪽창에서 값이 변화를 보여야한다.

7.In CE: Double click the value in the top, this adds it to the list on the bottom.

CE에서 : 상단의 값을 더블 클릭해서 하단의 리스트에 추가시킨다.

8.In CE: Right-click on the address on the bottom, click "find what writes to this address"

CE에서 : 하단의 주소를 우클릭하여 "find what writes to this address"를 클릭한다.

9.In game: Zoom in and out a few times, CE should update with an instruction in the new new window.

인게임에서 : 줌인과 줌아웃을 몇 차례 실행하여, CE의 새로운 새 창의 instruction으로 업데이트해야 한다.

10.In CE:

CE에서

11.Select the instruction

instruction 선택

12.Look for the line which does the writing, it will have '<<' at the end

쓸 수 있는 줄을 찾는다. 끝에 '<<'가 있을 것이다.

13.Look for the register and offset, you should see something like DX9: [ecx+000000F8], DX11: [r9+00000000000000F8] (note: it's been RCX before)

register와 offset을 찾는다. DX9라면 [ecx+000000F8], DX11이라면 [r9+00000000000000F8] 의 형식일 것이다. (이전에는 RCX였다.)

14.Find the address in the register, at the bottom look for ECX=0125BB80. Save this address, clipboard or notepad.

register에서 주소를 찾고, 하단에 ECX=0125BB80를 찾는다. 이 주소를 클립보드나 메모장에 저장해둔다.

15.Get back to the main CE window

CE 메인창으로 돌아온다.

16.In CE: Click "New Scan", Value Type DX9: 4 Bytes, DX11: 8 Bytes, check Hex. Search

CE에서 : "New Scan"을 클릭, Value Type을 DX9: 4 Bytes, DX11: 8 Bytes으로, Hex(16진수) 선택 후 검색.

17.In CE: Top list should show multiple results, for all green ones do this until something makes sense:

CE에서 : 상단 목록은 여러개의 결과가 나와야 하고, 모든 녹색의 무언가가 확실해질 때까지 이것을 실행해야 된다.

18.Double-click the address in the top

상단의 주소를 더블 클릭.

19.Double-click the address in the bottom that appears, make sure to click on the 'Address' value

하단에 나타난 주소를 더블 클릭하고 'Address' 값을 클릭했는지 확인한다.

20.Copy the address, DX9: ffxiv.exe+offset, DX11: ffxiv_dx11.exe+offset

주소를 복사하고 DX9: ffxiv.exe+offset, DX11: ffxiv_dx11.exe+offset

21.Check Pointer, change Type to Float

Check Pointer, Type을 Float으로 변경.

22.Paste the address in the box above "Add Offset", click OK

"Add Offset" 위의 상제에 주소를 붙여넣고 OK 클릭.

23.If the Value is displayed as a hex: Right-click the row in the bottom, click "show as decimal"

만약 값이 16진수로 표시될 경우 하단의 행을 우클릭 후 "show as decimal(10진수로 보기)" 클릭.

24.Ensure that value updates as you zoom

줌 할때 값이 업데이트 되는지 확인.
