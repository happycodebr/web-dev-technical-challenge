


const getPokemonUrl = id  => `https://pokeapi.co/api/v2/pokemon/${id}`


  const genneratePokemonPromises = () => Array(150).fill().map((_, index) =>
  fetch(getPokemonUrl(index + 1)).then(response => response.json()))

 const generateHtml = pokemons => pokemons.reduce((accumulator, {name, id, types}) => {
   const elementTypes = types.map(typeInfo => typeInfo.type.name)
 


        accumulator += `
        <li class="card" ${elementTypes[0]}">
        <img class=" card-image " alt="${name} " src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/${id}.png>",
        <h2 class="card-title">${id}.${name}</h2>
        <p  class="card-subtitle">${elementTypes.join(' / ')}</p>
        <br>
        <br>
        <input onclick="adicionar()"  type="adicionar" value="adicionar">
        <input onclick="remover()"    type="remover" value="remover">
         </li>
       
        `
        return accumulator
} ,'')


const insertPokemonsIntoPage = pokemons => {
    const ul = document.querySelector('[data-js="pokedex"]')
    ul.innerHTML = pokemons
}

  const pokemonPromises = genneratePokemonPromises() 
     Promise.all(pokemonPromises)
      .then(generateHtml)
      .then(insertPokemonsIntoPage)



    //enviar e-mail

  const enviaemail = require("enviaemail");

  let transporter = enviaemail.createTransport({
    host:"smtp.umbler.com",
    port:587,
    secure:false,
    auth:{
      user:"augusto,mota@unicesumar,edu.br",
      pass:"Asdqwe123@"
    }
    
  });


  transporter.sendMail({
    from: "augusto,mota@unicesumar,edu.br",
    to: "augusto,mota@unicesumar,edu.br",
    subject:"oi  Happy",
    Text:"Olá happy",
    html:"Olá "

  }).then(message =>{
    console.log(message);
  }).catch(err =>{
    console.log(err);
  })


  
function validar(){

  function validar() {

    var nome      = document.getElementById("nome");
    var sobrenome = document.getElementById("sobrenome");
    var email     = document.getElementById("email");
    var senha     = document.getElementById("senha");

    //  nome está vazio
  if (nome.value == "") {
    alert("Nome não informado");

    //  focus

    nome.focus();
    
    
    // retorna a função 
    return;
  }
  if (sobrenome.value == "") {
    alert("Sobrenome não informado");
    sobrenome.focus();
    return;
  }
  if (email.value == "") {
    alert("E-mail não informado");
    email.focus();
    return;
  }
  if (senha.value == "") {
    alert("Senha não informada");
    senha.focus();
    return;
  }
  
  
}

alert("Formulário enviado!");

}


// adicionar pokemon contrutor 

class pokemon {
  constructor(name, id, types) {
      this.name = name;
      this.id = id;
      this.types = types;
  }
}



function adicionar(){
  var pokemonid     = document.getElementById("pokemonid ");

}

function remover(){

  var pokemonid     = document.getElementById("pokemonid ");

}

function buscar(){



}

