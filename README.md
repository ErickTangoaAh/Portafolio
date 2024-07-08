<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>Encriptador de texto</title>
  </head>
  <body>
    <main class="main">
      <section class="main__section--encriptador">
        <textarea id="textoEntrada" class="encriptador__textarea--encriptar" placeholder="Ingrese el texto aquí"></textarea>
        <div class="encriptador__mensaje">
          <p class="encriptador__alert-text">Ingrese solo letras minúsculas y sin acentos.</p>
        </div>
        <div class="encriptador__buttons">
          <button id="botonEncriptar" class="main__buttons encriptador__button--encriptar" onclick="encriptarTexto();">Encriptar</button>
          <button id="botonDesencriptar" class="main__buttons encriptador__button--desencriptar" onclick="desencriptarTexto()">Desencriptar</button>
        </div>
      </section>
      <section class="main__section--resultado">
        <textarea id="textoResultado" class="resultado__textarea--desencriptar" style="display: none;"></textarea>
        <img id="resultadoMunieco" src="img/Muñeco.png" alt="imagen de Muñeco" class="resultado__munieco">
        <div id="resultadoInformacion" class="resultado__informacion">
          <p class="resultado__texto-negrita">Ningún mensaje fue encontrado</p>
          <p class="resultado__texto-mensaje">Ingresa el texto que desees encriptar o desencriptar.</p>
        </div>
        <span id="mensajeCopiado" class="resultado__texto-copiado" style="display: none;">Texto copiado!</span>
        <button id="botonCopiar" class="main__buttons resultado__button--copiar" onclick="copiarTexto();" style="display: none;">Copiar</button>
      </section>      
    </main>
    <footer class="footer">
      <p class="footer__informacion"> Erick Tangoa Alura 2024 </p>
    </footer>
    <script src="app.js"></script>
  </body>
</html>
