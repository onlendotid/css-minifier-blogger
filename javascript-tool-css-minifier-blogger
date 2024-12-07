function minifyCSS() {
    var input = document.getElementById('inputCSS').value;
    var output = input.replace(/\s+/g, ' ')
                      .replace(/\/\*[^*]*\*+([^/][^*]*\*+)*\//g, '')
                      .replace(/\s*{\s*/g, '{')
                      .replace(/\s*}\s*/g, '}')
                      .replace(/\s*:\s*/g, ':')
                      .replace(/\s*;\s*/g, ';')
                      .replace(/;\}/g, '}');
    document.getElementById('outputCSS').value = output;
  }

  function beautifyCSS() {
    var input = document.getElementById('inputCSS').value;
    var formatted = input.replace(/;/g, ';\n  ')
                         .replace(/{/g, ' {\n  ')
                         .replace(/}/g, '\n}\n')
                         .replace(/ {2,}/g, ' ')
                         .trim(); 
    document.getElementById('outputCSS').value = formatted;
  }

  function copyOutput() {
    var output = document.getElementById('outputCSS');
    output.select();
    output.setSelectionRange(0, 99999);
    document.execCommand('copy');
    alert('Kode berhasil disalin!');
  }

  function clearOutput() {
    document.getElementById('inputCSS').value = '';
    document.getElementById('outputCSS').value = '';
  }
