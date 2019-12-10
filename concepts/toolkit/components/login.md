---
title: Componente de logon no kit de ferramentas do Microsoft Graph
description: Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 767894cc88fa40eb96655fc8979dd5b2ef8d4eba
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39919434"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Componente de logon no kit de ferramentas do Microsoft Graph

Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft. Ele fornece dois Estados:
* Quando o usuário não está conectado, o controle é um botão simples para iniciar o processo de entrada.
* Quando o usuário está conectado, o controle exibe o nome de usuário conectado atual, a imagem de perfil e o email. Quando clicado, um submenu é aberto com um comando para sair.

## <a name="example"></a>Exemplo

[exemplo de jsfiddle](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a>Usando o controle sem um provedor de autenticação

O componente funciona com um provedor e o Microsoft Graph. No entanto, se você quiser fornecer sua própria lógica e autenticação, você pode usar `userDetails` a propriedade para definir os detalhes do usuário conectado. 

| Atributo | Propriedade | Descrição |
| --- | --- | -- |
| User-detalhes | userdetails | Defina o objeto de usuário que será exibido no controle. |

O exemplo a seguir define os detalhes da pessoa.

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

A `userDetails` configuração `null` para vai para o estado de desconectar.

Use os `loginInitiated` eventos `logoutInitiated` e para lidar com a entrada e a saída. 

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-login` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --color-hover: var(--theme-primary-color);
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

Para saber mais, confira [estilos de componentes](../style.md).

## <a name="events"></a>Eventos

Os eventos a seguir são acionados do controle.

| Evento | Descrição |
| --- | --- |
| `loginInitiated` | O usuário clicou no botão entrar para iniciar o processo de logon-cancelable.|
| `loginCompleted` | o processo de login foi bem-sucedido e o usuário está conectado. |
| `loginFailed` | O usuário cancelou o processo de logon ou não pôde entrar.|
| `logoutInitiated` | O usuário iniciou o logout-cancelamento. |
| `logoutCompleted` | O usuário saiu. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões. 

## <a name="authentication"></a>Autenticação

O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md). 
