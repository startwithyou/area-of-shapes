# area-of-shapes
<html>
  <head>
    <title>The area of a triangle</title>
    <h1>Calculating Area using JavaScript</h1>
    <list>
      <button onclick="area_triangle()" id="btnl">traingle</button>
      <button onclick="area_rectangle()" id="btnl">rectangle</button>
      <button onclick="area_circle()" id="btnl">circle</button>
    </list>
    <script>
      function area_triangle() {
        var side1 = parseInt(prompt("Enter side1 in cm"));
        var side2 = parseInt(prompt("Enter side2 in cm"));
        var side3 = parseInt(prompt("Enter side3 in cm"));
        var s = (side1 + side2 + side3) / 2;
        var area = Math.sqrt(s * ((s - side1) * (s - side2) * (s - side3)));
        console.log(
          "<br>" + "Area of triangle is = " + area.toFixed(2) + "sq.cm."
        );
        document.write(
          "<br>" + "Area of triangle is = " + area.toFixed(2) + "sq.cm."
        );
      }
      function area_rectangle() {
        var side1 = parseInt(prompt("Enter side1"));
        var side2 = parseInt(prompt("Enter side2"));
        var area = side1 * side2;
        console.log(
          "<br>" + "Area of triangle is = " + area.toFixed(2) + "sq.cm."
        );
        document.write(
          "<br>" + "Area of rectangle is = " + area.toFixed(2) + "sq.cm."
        );
      }
      function area_circle() {
        var radius = parseInt(prompt("Enter radius"));
        var area = 3.14 * radius * radius;
        console.log(
          "<br>" + "Area of triangle is = " + area.toFixed(2) + "sq.cm."
        );
        document.write(
          "<br>" + "Area of circle is = " + area.toFixed(2) + "sq.cm."
        );
      }
    </script>
  </head>
</html>
