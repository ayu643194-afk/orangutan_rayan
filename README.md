        <img src="https://placehold.co/600x400?text=Generated+Image" alt="Generated Image"/>
      `;
    }

    function generateVeo() {
      let prompt = document.getElementById("veoPrompt").value;
      let result = document.getElementById("veoResult");
      if(prompt.trim() === "") {
        result.innerHTML = "<p style='color:red'>⚠️ Harap isi prompt VEO!</p>";
        return;
      }
      // Output contoh format prompt
      result.innerHTML = `
        <p><strong>Prompt VEO 3:</strong></p>
        <pre>
          {
            "version": "VEO-3",
            "scene": [
              {
                "description": "${prompt}",
                "style": "realistic, cinematic, 4K",
                "camera": "dynamic shot, smooth transition"
              }
            ]
          }
        </pre>
      `;
    }
  </script>
</body>
</html>
