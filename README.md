# SI_2022_lab2_111098

Vladimir Jovanovski 111098

<h2><b>Control Flow Graph</b><h2>
![cfg_vladimir](https://user-images.githubusercontent.com/100305400/171938351-21f2ef2a-c9c0-4acb-ac38-e31ec693e9c9.png)



  
<h2><b>Цикломатска комплексност</b></h2>
Цикломатската комплексност на овој код е 9. Оваа комплексност ја добив со помош на следната формула:</br>
  <b>E-N+2=C</b></br>
  N=23</br>
  E=30</br>
  C = 30-23+2</br>
  C = 9</br>
  
<h2><b>Тест случаи според критериумот Every statement</b></h2>
1. input -> {} , output -> throw exception, nodes -> 1,2 ,3 ,24 </br>
- тест случајов врши проверка на ф-јата ако се прати некоја листа која е празна </br>
2. input -> {"#", "#", "0", "0", "0"}, output -> throw exeption, nodes -> 1,2 ,4,5 ,6 ,7 ,24 </br>
- низата која е пратена како параметар во оваа ф-ја врши проверка на правилото да биде успешно изврешна. </br>
3. input -> {"0", "#", "0", "#", "#", "0", "#", "0", "0", "#", "0", "#", "#", "0", "0", "0"},</br>
   output ->{"2", "#", "3", "#", "#", "4", "#", "3", "3", "#", "3", "#", "#", "2", "0", "1"},</br>
   nodes -> from 1,2 to 24</br>
- целта на овој тест случај е да се изминат сите кејсови без грешка
   
<h2><b> Тест случаи според критериумот Every branch</b></h2>

1. input -> {} , output -> throw exception,
2. input -> {"#", "#", "0", "0", "0"}, output -> throw exeption,
3. input -> {"0", "#", "0", "#", "#", "0", "#", "0", "0", "#", "0", "#", "#", "0", "0", "0"},</br>
   output ->{"2", "#", "3", "#", "#", "4", "#", "3", "3", "#", "3", "#", "#", "2", "0", "1"},</br>
 
 - За Every Branch се реискористуваат тест случаеви што се користат во Every Statement.
 - со третиот тест случај се постигнува со еден тест кејс да ги исполни сите можни гранки и нивите исходи</br> без да настане грешка
 
 <table>
  <tr>
    <th>Branches</th>
    <th>Case 1</th>
    <th>Case 2</th>
    <th>Case 3</th>
  </tr>
  <tr>
    <td> 1,2 - 3</td>
    <td>*</td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td>1,2- 4,5</td>
    <td></td>
    <td>*</td>
    <td>*</td>
  </tr>
  <tr>
    <td> 6 - 7</td>
    <td></td>
    <td>*</td>
    <td></td>
  </tr>
    <tr>
    <td>6 - 8</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
     <td>9.2 - 23</td>
     <td></td>
     <td></td>
     <td></td>
  </tr>
   <tr>
    <td>9.2 - 10</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>10 - 21</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>10 - 11,12</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>11,12 - 13</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>11,12 - 16</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>13 - 14</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>13 - 15</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>16 - 17</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>16 - 18</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>18 - 19</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
   <tr>
    <td>18 - 20</td>
    <td></td>
    <td></td>
    <td>*</td>
  </tr>
</table> 
