---
title: Componente de logon no kit de ferramentas do Microsoft Graph
description: Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 441639c309025eb8fefbbe551dd60b6324a7fd3c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682030"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Componente de logon no kit de ferramentas do Microsoft Graph

Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft. Ele fornece dois Estados:
* Quando o usuário não está conectado, o controle é um botão simples para iniciar o processo de entrada.
* Quando o usuário está conectado, o controle exibe o nome de usuário conectado atual, a imagem de perfil e o email. Quando clicado, um submenu é aberto com um comando para sair.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-login` componente com um usuário conectado. 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a>Usando o controle sem um provedor de autenticação

O componente funciona com um provedor e o Microsoft Graph. No entanto, se você quiser fornecer sua própria lógica e autenticação, você pode usar a `userDetails` propriedade para definir os detalhes do usuário conectado. 

| Atributo | Propriedade | Descrição |
| --- | --- | -- |
| User-detalhes | userdetails | Defina o objeto de usuário que será exibido no controle. |

O exemplo a seguir define os detalhes da pessoa.

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

`userDetails`A configuração para vai `null` para o estado de desconectar.

Use os `loginInitiated` `logoutInitiated` eventos e para lidar com a entrada e a saída. 

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

## <a name="templates"></a>Modelos

O `mgt-login` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos valores listados na tabela a seguir. 

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| conectado ao botão de conteúdo | personDetails: objeto Person, `personImage` : cadeia de caracteres de imagem de pessoa | O modelo usado para renderizar o conteúdo no botão quando o usuário está conectado. |
| desconectado-botão-conteúdo | null | O modelo usado para renderizar o conteúdo no botão quando o usuário não está conectado. |
| submenu-comandos | handleSignOut: função de saída | O modelo usado para renderizar os comandos no submenu |
| submenu de pessoas-detalhes | personDetails: objeto Person, personImage: cadeia de caracteres de imagem de pessoa | O modelo usado para renderizar os detalhes da pessoa no submenu. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões. 

## <a name="authentication"></a>Autenticação

O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md). 

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.

| Método | Descrição |
| - | - |
| renderButton | Renderiza o cromo do botão. |
| renderButtonContent | Renderiza o conteúdo do botão. |
| renderSignedInButtonContent | Processe o conteúdo do botão quando o usuário estiver conectado. |
| renderSignedOutButtonContent | Renderiza o conteúdo do botão quando o usuário não está conectado. |
| renderFlyout | Renderiza o cromo domenu. |
| renderFlyoutContent | Renderiza o conteúdo do submenu. |
| renderFlyoutPersonDetails | Renderizar os detalhes da pessoa de submenu. |
| renderFlyoutCommands | Renderizar os comandos de submenu. |

### <a name="bring-your-own-flyout"></a>Traga seu próprio submenu

É possível usar seu próprio componente de submenu no lugar do interno, substituindo o `renderFlyout()` método e fornecendo o novo submenu.

Nesse caso, verifique se o componente de login continua funcionando conforme o esperado, substituindo os `protected` métodos de exibição de submenu para atualizar a visibilidade do submenu alternativo.

| Método | Descrição |
| - | - |
| hideFlyout | Descarta o submenu. |
| Menu de atalho | Exibe o submenu. |
| toggleFlyout | Alterna o estado do submenu. |
