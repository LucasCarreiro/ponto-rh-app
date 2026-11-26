# Ponto RH

Aplicativo mobile de **ponto eletrônico** em React Native: o colaborador cria a conta, entra e registra o ponto com horário e localização. Os dados ficam salvos no próprio aparelho, em SQLite.

## Funcionalidades

- Cadastro e login, com senha guardada em hash SHA-256
- Registro de ponto com horário (seletor de data e hora) e geolocalização
- Validação dos formulários
- Navegação entre as telas com React Navigation
- Persistência local com SQLite

## Estrutura

```
App.js                              navegação entre as telas
src/screens/LoginScreen.js          login
src/screens/SignUpScreen.js         cadastro
src/screens/ClockInScreen.js        registro de ponto
src/screens/src/components/TimePickerModal.js
src/database/db.js                  conexão e criação das tabelas SQLite
src/database/models/User.js         usuários
src/database/models/Point.js        registros de ponto
```

## Como rodar

Pré-requisitos: ambiente React Native configurado (Android Studio ou Xcode).

```bash
npm install
npx react-native run-android   # ou: npx react-native run-ios
```

O acesso à localização é solicitado com `react-native-permissions`.

## Tecnologias

React Native · React Navigation · SQLite (`react-native-sqlite-storage`) · `react-native-geolocation-service` · `react-native-sha256` · `@react-native-community/datetimepicker`

---

Feito por **Lucas Carreiro** · [LinkedIn](https://www.linkedin.com/in/lucas1carreiro1/)
