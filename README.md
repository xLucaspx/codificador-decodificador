# Codificador e Decodificador de texto
## Utilizando HTML, CSS e JavaScript
Este é um projeto desenvolvido durante o programa **ONE - Oracle Next Education**; é o primeiro *challenge* disponibilizado, com o objetivo de colocar em prática os conteúdos estudados.
<br>
O desafio consiste em criar um **codificador/decodificador** de texto utilizando conhecimentos em **HTML**, **CSS** e **JavaScript** adquiridos durante as aulas.
Foram disponibilizados *cards* no *Trello* para orientar e gerenciar o desenvolvimento do projeto e um modelo proposto de estilização no *Figma*.
### Meu projeto
Sempre tento manter meu código o mais organizado possível, para facilitar a compreensão e o acesso, caso algo precise ser alterado.
<br>
**Na estrutura HTML modifiquei:**
- o *header*, onde coloquei o *link* da página no logo. Assim, ao clicar no logo, a página é recarregada (eu geralmente faço isso pois acho uma funcionalidade interessante);
- o aviso de "apenas letras minúsculas e sem acento" para aparecer somente se o usuário digitar letras maiúsculas ou acentuadas;
- a *textarea* que mostra o resultado da codificação/decodificação para ***readonly***, pois caso o usuário digitasse algo algo nela (com ou sem intenção) e depois tentasse fazer a codificação/decodificação, o texto não era mostrado;
- o *footer*, onde adicionei meu nome e redes sociais; <br><br>
**No CSS modifiquei:**
- A fonte para *"Montserrat light 300"*, seu tamanho e o espaçamento das linhas;
- As cores do fundo (com um gradiente de azul-claro para azul-escuro) e das sombras;
- As animações dos *links* e dos botões (usei ***transform*** e ***opacity***);
- O ponto de exclamação antes das mensagens de erro (***::before***) e a imagem de fundo da *textarea* quando não há texto inserido (***:placeholder-shown***);
- O *layout* da página para dispositivos com até *480px* de largura; <br><br>
**No JavaScript:**
- Criei a função de codificar separando os caracteres do texto em um *array* (***texto.value.split***), substituindo com ***forEach*** e retornando com ***.join("")***;
- Criei a função de decodificar utilizando um *array* com a "chave" da codificação e utilizando ***replaceAll(chave[ i ][ 1 ])***;
- Criei uma função para validar o texto inserido, permitindo apenas letras minúsculas e sem acento;
- Criei uma fução para mostrar uma mensagem de erro caso não fosse inserido texto;
- Criei uma função para que, ao copiar o texto codificado/decodificado usando o botão "copiar", as *textareas* sejam limpas e o input seja focado, para que o usuário não precise novamente clicar no input e apagar o texto previamente digitado para colar outro texto.
