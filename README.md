# Conversor de Moeda

Um aplicativo simples de conversão de moeda desenvolvido em React Native. O aplicativo permite que os usuários convertam valores entre diferentes moedas, utilizando uma API para obter as taxas de câmbio em tempo real.

## Funcionalidades

- Conversão entre várias moedas (USD, EUR, BRL, GBP, JPY, CAD)
- Exibição da taxa de câmbio atual entre as moedas
- Interface intuitiva e responsiva
- Animações suaves ao pressionar o botão de conversão
- Validação de entrada para evitar valores nulos e inválidos

## Tecnologias Utilizadas

- [React Native](https://reactnative.dev/)
- [Axios](https://axios-http.com/)
- [@react-native-picker/picker](https://github.com/react-native-picker/picker)

## Pré-requisitos

Antes de executar o projeto, você precisará ter o Node.js e o Expo CLI instalados em seu sistema. Você pode instalar o Expo CLI globalmente usando o seguinte comando:

```bash
npm install -g expo-cli
```

## Como Executar o Projeto

1. Clone o repositório:

   ```bash
   git clone https://github.com/thonyydev/ConversorMoeda.git
   cd ConversorMoeda
   ```

2. Instale as dependências:

   ```bash
   npm install
   ```

3. Execute o aplicativo:

   ```bash
   npm start
   ```

   Isso abrirá o Expo Dev Tools em seu navegador. Você pode escanear o código QR com o aplicativo Expo Go em seu dispositivo móvel para visualizar o aplicativo.

## Configuração da API

O aplicativo utiliza a API `exchangerate-api.com` para obter as taxas de câmbio. Você pode precisar adicionar sua própria chave de API. Substitua a chave da API no arquivo `App.js`:

```javascript
const response = await axios.get(`https://api.exchangerate-api.com/v4/latest/${fromCurrency}`, {
  headers: {
    'apikey': 'SUA_CHAVE_API_AQUI'  // Substitua com sua chave de API
  }
});
```

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões ou melhorias, sinta-se à vontade para abrir um Pull Request ou relatar um problema.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

## Contato

Se você tiver alguma dúvida, entre em contato:

- Nome: Thony
- GitHub: [thonyydev](https://github.com/thonyydev)
