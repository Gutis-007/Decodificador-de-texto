


# Codificador e Decodificador de Texto

Este é um projeto simples de codificador e decodificador de texto desenvolvido em JavaScript. O objetivo deste projeto é permitir que os usuários insiram um texto e escolham codificar ou decodificar esse texto usando uma interface web intuitiva.

## Funcionalidades

- **Codificação de Texto**: Converte o texto de entrada em um formato codificado.
- **Decodificação de Texto**: Converte o texto codificado de volta ao seu formato original.
- **Interface Intuitiva**: Uma interface amigável onde os usuários podem facilmente alternar entre codificação e decodificação.
- **Botão para Copiar Texto**: Um botão que permite aos usuários copiar o texto resultante diretamente para a área de transferência usando a Clipboard API.

## Como Usar

1. **Clone o Repositório**
   ```bash
   git clone https://github.com/gutis-007/Decodificador-de-texto.git
   ```
2. **Navegue até o Diretório do Projeto**
   ```bash
   cd Decodificador-de-texto
   ```
3. **Abra o `index.html` em seu Navegador Preferido**
   ```bash
   open index.html
   ```

## Clipboard API

Este projeto utiliza a Clipboard API para fornecer uma maneira fácil de copiar o texto resultante para a área de transferência. A Clipboard API é uma interface moderna e segura que permite copiar texto para a área de transferência do sistema diretamente do navegador. Abaixo está um exemplo de como isso foi implementado:

```javascript
function copyToClipboard() {
    const resultText = document.getElementById('resultText');
    navigator.clipboard.writeText(resultText.value).then(function() {
        alert('Texto copiado para a área de transferência!');
    }, function(err) {
        console.error('Erro ao copiar texto: ', err);
    });
}

document.getElementById('copyButton').addEventListener('click', copyToClipboard);
```

## Deploy

O projeto foi implantado no GitHub Pages e pode ser acessado pelo seguinte URL: [Decodificador de Texto](https://gutis-007.github.io/Decodificador-de-texto/).

## Contribuição

Sinta-se à vontade para contribuir com este projeto. Para isso, siga os passos abaixo:

1. **Fork o Repositório**
2. **Crie uma Branch para sua Funcionalidade (git checkout -b feature/nova-funcionalidade)**
3. **Commit suas Mudanças (git commit -m 'Adiciona nova funcionalidade')**
4. **Push para a Branch (git push origin feature/nova-funcionalidade)**
5. **Abra um Pull Request**

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

Este arquivo Markdown contém todas as seções necessárias para descrever seu projeto, incluindo funcionalidades, instruções de uso, detalhes sobre a utilização da Clipboard API, o link para o GitHub Pages onde o projeto está hospedado e informações sobre como contribuir e a licença do projeto.
