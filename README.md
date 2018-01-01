# HTML5 Canvas to image converter
JS Libraries used html2canvas converter and canvas2image converter


      html2canvas($("#widget"), { 
            onrendered: function(canvas) {
                theCanvas = canvas;
                document.body.appendChild(canvas);
                
                // Convert and download as image 
                Canvas2Image.saveAsPNG(canvas); 
                $("#img-out").append(canvas);
                // Clean up 
                //document.body.removeChild(canvas);
            }
        });
