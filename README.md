1.In CE: File - Open process. for DX9: ffxiv.exe, DX11: ffxiv_dx11.exe

CE에서 : 프로세스 열기 (DDX9: ffxiv.exe, DX11: ffxiv_dx11.exe)

2.In game: Zoom all the way out, make sure there are no obstructions

인게임에서 : 장애물 없이 끝까지 줌 아웃

3.In CE: On the right side, change Value Type to Float. Look for Value 20.0

CE에서 : 오른쪽에서 Value Type을 Float로 변경, 값 20.0을 찾는다.

4.In game: Zoom all the way in without going to first person

인게임에서 : 1인칭 사용하지 않고 끝까지 줌 인

5.In CE: Change Value to 1.5, hit enter or click "Next Scan"

CE에서 : 값을 1.5로 변경, 엔터 or 클릭으로 "Next Scan"

6.Repeat steps 2-5 until you see the value of interest in the window on the left. You should see the value changing as you change zoom in game.

7.In CE: Double click the value in the top, this adds it to the list on the bottom.

8.In CE: Right-click on the address on the bottom, click "find what writes to this address"

9.In game: Zoom in and out a few times, CE should update with an instruction in the new new window.

10.In CE:

11.Select the instruction

12.Look for the line which does the writing, it will have '<<' at the end

13.Look for the register and offset, you should see something like DX9: [ecx+000000F8], DX11: [r9+00000000000000F8] (note: it's been RCX before)

14.Find the address in the register, at the bottom look for ECX=0125BB80. Save this address, clipboard or notepad.

15.Get back to the main CE window

16.In CE: Click "New Scan", Value Type DX9: 4 Bytes, DX11: 8 Bytes, check Hex. Search

17.In CE: Top list should show multiple results, for all green ones do this until something makes sense:

18.Double-click the address in the top

19.Double-click the address in the bottom that appears, make sure to click on the 'Address' value

20.Copy the address, DX9: ffxiv.exe+offset, DX11: ffxiv_dx11.exe+offset

21.Check Pointer, change Type to Float

22.Paste the address in the box above "Add Offset", click OK

23.If the Value is displayed as a hex: Right-click the row in the bottom, click "show as decimal"

24.Ensure that value updates as you zoom
