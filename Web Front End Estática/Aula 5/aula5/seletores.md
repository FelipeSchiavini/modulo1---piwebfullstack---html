# Seletores do CSS

Operador > Quando um elemento está diretamente dentro de outro

exemplo:

section > h2

<section>
  <h2></h2>
</section>

"Espaço" quando um elemento está dentro do outro em qualquer posição

section h2
ou
section > div > h2

<section>
  <div>
    <h2></h2>
  </div>
</section>

Operador + quando um elemento sucede outro

section h2 + h2

section > div > h2 + h2

<section>
  <div>
    <h2>Título um</h2>
    <h2>Título dois</h2>
  </div>
</section>

Operador nth-child(n) especifique n para selecionar o elemento escolhido (evite usar pois pode dar problemas de manutenção no seu código)

Mesma operação que section h2 + h2 no caso abaixo:
section h2:nth-child(2)

<section>
  <div>
    <h2>Título um</h2>
    <h2>Título dois</h2>
  </div>
</section>

Contudo, não funcionaria corretamente para o seguinte caso:
section h2:nth-child(2)

mas funcionaria
section h2 + h2

<section>
  <div>
    <img src="qualquercoisa.jpg" alt="qualquer alt" />
    <h2>Título um</h2>
    <h2>Título dois</h2>
  </div>
</section>
