DELA CRUZ, Johann Sebastian A. 9-Li
1. js line 1, plotPoint() - no parameters, arguments are passed thru HTML, changed to function plotPoint(x0, y0, x, y)
2. js line 2, console.log(x0, y0, x, y) - undefined, fixed by adding parameters to plotPoint
3. js line 3, in1 - undefined, fixed by adding var in1 = document.getElementById("in1");
4. js line 12, 15, 18, 21, 24, out1 - undefined, fixed by adding var out1 = document.getElementById("out1");
5. js line 6, point.styleleft - syntax error, edited to point.style.left
6. js line 7, point.stylebottom - syntax error, edited to point.style.bottom
7. js line 25, missing closed brace
8. CSS line 38, a :hover - space makes error, removed space, --- a:hover
9. CSS line 31, a display:block;, stacks link vertically, changed to display:inline-block;
10. CSS line 25, added position: fixed; top: 0; left: 0; 
