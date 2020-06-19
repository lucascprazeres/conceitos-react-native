![gostack](.github/gostack.png)

<h1 align="center">
  🚀Conceitos React Native🚀

  <p align="center">
  <img src="https://img.shields.io/badge/tech-mobile-ff69b4" />

  <a href="https://reactjs.org/">
    <img src="https://img.shields.io/badge/framework-React%20Native-brightgreen" />
  </a>

  <a href="https://github.com/Rocketseat">
    <img src="https://img.shields.io/badge/source-rocketseat-blueviolet" />
  </a>
  </p>
</h1>


<p>
  Esse app é o cliente mobile que consome a api construída <a href="https://github.com/lucascprazeres/conceitos-nodejs">nesse desafio</a>. Com suporte para listar e curtir os repositórios fake.
</p>

<h2 align="center">
  Sobre 🕵️
</h2>

<p>
  O quarto desafio prático do bootcamp goStack trouxe os fundamentos do React Native, de forma prática, visando consumir a api construída no desafio citado acima. É importante que os devs não familiarizados com essa tecnologia deem uma olhada no arquivo <em>src/app</em>, para entender as diferenças em relação ao React, em sua <a href="https://github.com/lucascprazeres/conceitos-reactjs">versão web</a>.
</p>

<h2 align="center">
  ReactJS e React Native... Tem diferença? 🤔💭
</h2>

<p align="center">
  <strong>Sim!</strong> Apesar de ambas as tecnologias fazerem parte do ecossistema React, e de suas implementações serem bastante semelhantes, elas têm algumas diferenças, em seu uso.
</p>

<ul>
  <li>
    <strong>Sem tags HTML ou css</strong>!: Como o React Native não constrói interfaces híbridas, mas nativas, as tags html e o próprio css não funcionam aqui!
  </li>
  <li>
    <strong>Seus próprios componentes</strong>: A boa notícitia, pra que se desanimou com o último item, é que as tags são utlizadas da mesma forma! Porém, temos de utilizar componentes nativos, como base.

  ```javascript
    import React from 'react';  //  ainda é necessário fazer isso
    import { View, Text, TouchableOpacity } from 'react-native';

    function App() {
      return (
        <View> {/* É um container genérico, como uma div, span, aside, section e etc... */}
          <Text>  {/* TODO tipo de texto precisa ser inserido dentro dessa tag de texto genérica */}
            Hello, World!  
          </Text>

          <TouchableOpacity> {/* Apenas um, dos inúmeros botões disponíveis */}
            Me Pressione!
          </TouchableOpacity>
        </View> 
      );
    }
  ```
  </li>
  <li>
    <strong>Estilizando componentes</strong>: uma das formas de estilizar componentes dentro do React Native é utilizando o StyleSheet. Lembra da sintaxe que você já utilizava no css? Ainda está aqui!

  ```javascript
    // ... outros imports
    import { View, Text, StyleSheet } from 'react-native';

    function App() {
      return (
        <View style={styles.container}>
          <Text style={styles.title}>
            Esse vai ser o título da minha página!
          </Text>
        </View>
      );
    }

    const styles = StyleSheet.create({
      container: {
        flex: 1,
      },
      title: {
        fontSize: 32,
        color: '#7159c1'
      }
    });
  ```
  <p>
    <em>
      Masss, antes de sair codando, lembre-se de duas coisas: Aqui, não há estilização por cascata. Ou seja, Se eu quisesse alterar a cor do meu título, teria de fazer isso em diretamente em title, não em container. Além disso, a propriedade 'display: "flex"', já é definida por padrão, em todos os componentes!
    </em>
  </p>
  </li>
</ul>


<h2 align="center">
  Quero testar o app!
</h2>

```bash
  #  clone o repositório
  git clone link-do-repositorio

  #  navegue até o repositório clonado
  cd conceitos-reactjs

  #  baixe as dependências
  yarn

  #  divirta-se!
  yarn start
```

<h2 align="center">
  Não seria melhor se...
</h2>

<p>
  Se você deseja sugerir alguma mudança, basta fazer o seguinte:

```bash
  #  execute os mesmos passos da sessão anterior, mas dessa vez, crie a sua branch
  git checkout -b minha-branch

  # faça commit  das suas alterações e, em seguida, realize um pull request
  git add .
  git commit -m 'eu mudei...'
  git push origin master

  # Assim, eu vou poder adicionar as suas mudanças ao projeto!
```
<p>

<h2 align="center">
  Curtiu o conteúdo? 😍
</h2>

<p align="center">
  Avalie o reposiorio com uma ⭐ para que outros devs possam encontrá-lo!<br>
  Além disso, você pode encontrar esse repositório mais facilmente 💜🚀
<p>

***

<p align="center">
  Feito com muito 💜 por <a href="https://www.linkedin.com/in/lucas-prazeres/">Lucas dos Prazeres</a>
</p>