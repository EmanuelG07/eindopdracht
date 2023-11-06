const prompt = require('prompt-sync')(); 

console.log("Welkom bij het keuzeverhaal!");
console.log("Je staat voor een kruispunt. Welke kant ga je op?");

const keuze = prompt("Kies een optie: links (L) of rechts (R): ");

if (keuze === "L" || keuze === "l") {
  console.log("Je gaat naar links en komt bij een donkere grot.");
  const grotOptie = prompt("Ga je de grot in (I) of blijf je buiten (O)? ");

  if (grotOptie === "I" || grotOptie === "i") {
    console.log("Je gaat de grot in en ontdekt een schat!");
  } else if (grotOptie === "O" || grotOptie === "o") {
    console.log("Je besluit buiten te blijven en gaat verder op je avontuur.");
  } else {
    console.log("Ongeldige keuze, het verhaal eindigt hier.");
  }
} else if (keuze === "R" || keuze === "r") {
  console.log("Je gaat naar rechts en komt bij een brug over een diepe kloof.");
  const brugOptie = prompt("Steek je de brug over (S) of ga je terug (T)? ");

  if (brugOptie === "S" || brugOptie === "s") {
    console.log("Je steekt de brug over en bereikt de overkant veilig.");
  } else if (brugOptie === "T" || brugOptie === "t") {
    console.log("Je besluit om terug te keren en verkent een andere route.");
  } else {
    console.log("Ongeldige keuze, het verhaal eindigt hier.");
  }
} else {
  console.log("Ongeldige keuze, het verhaal eindigt hier.");
}

console.log("Bedankt voor het spelen van het keuzeverhaal!");
