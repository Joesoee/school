<!DOCTYPE html>
<html>
    <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
    <!-- we import arjs version without NFT but with marker + location based support -->
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
    <body style="margin : 0px; overflow: hidden;">
        <a-scene embedded arjs="trackingMethod: best; debugUIEnabled: false; detectionMode: mono_and_matrix; matrixCodeType: 3x3;">
           <a-assets>
    <img id="my-image" src="picture.jpeg">
  </a-assets>

      <a-marker preset="hiro">
                <a-text value="Antwoord-1" color="red" rotation="-90 0 0"  scale="2 2 2"></a-text>
                          <a-text value="Antwoord-1" color="red" rotation="-90 10 0"  scale="2 2 2"></a-text>

            </a-marker>
            <a-marker type='barcode' value='2'>
                <a-text value="Opdracht 2!" color="blue" rotation="-90 0 0"  scale="2 2 2"></a-text>
            </a-marker>
            <a-marker type='barcode' value='3'>
                <a-text value="Opdracht 3!" color="green" rotation="-90 0 0"  scale="2 2 2"></a-text>
            </a-marker>
            <a-marker type='barcode' value='4'>
                <a-text value="Opdracht 4!" color="yellow" rotation="-90 0 0"  scale="2 2 2"></a-text>
            </a-marker>
            <a-marker type='barcode' value='5'>
                <a-text value="Opdracht 5!" color="orange" rotation="-90 0 0"  scale="2 2 2"></a-text>
            </a-marker>
            <a-marker type='barcode' value='6'>
  <a-image src="#my-image" rotation="-90 0 0"  scale="2 2 2"></a-image>
            </a-marker>
            <a-marker type='barcode' value='7'>
                <a-text value="Opdracht 7!" color="black" rotation="-90 0 0"  scale="2 2 2"></a-text>
        </a-marker>
        <a-entity camera></a-entity>
        </a-scene>
    </body>
</html>
