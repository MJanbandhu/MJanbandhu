<p align="center">
    <span id="rotatedName"></span>
</p>
<p align="center">
    Certified Data Scientist
</p>

<script>
// Function to rotate alphabet
function rotateAlphabet(text, shift) {
    let result = "";
    for (let i = 0; i < text.length; i++) {
        let charCode = text.charCodeAt(i);
        if (charCode >= 65 && charCode <= 90) {
            result += String.fromCharCode(((charCode - 65 + shift) % 26) + 65);
        } else if (charCode >= 97 && charCode <= 122) {
            result += String.fromCharCode(((charCode - 97 + shift) % 26) + 97);
        } else {
            result += text[i];
        }
    }
    return result;
}

// Rotate the name "Mohit Janbandhu" by 1 position
document.getElementById("rotatedName").innerText = rotateAlphabet("Mohit Janbandhu", 1);
</script>
