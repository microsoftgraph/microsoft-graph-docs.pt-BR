---
title: Componente de logon no microsoft Graph Toolkit
description: Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5dd610407fde25089a9c323b6b0cfb7965d33671
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334763"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Componente de logon no microsoft Graph Toolkit

Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação. Ele fornece dois estados:
* Quando o usuário não está assinado, o controle é um botão simples para iniciar o processo de logoff.
* Quando o usuário está assinado, o controle exibe o nome de usuário, a imagem do perfil e o email. Quando clicado, um sobrevoo é aberto com um comando para sair.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra `mgt-login` o componente com um usuário internado. 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a>Usando o controle sem um provedor de autenticação

O componente funciona com um provedor e a Microsoft Graph fora da caixa. No entanto, se você quiser fornecer sua própria lógica e autenticação, poderá usar a propriedade para definir os detalhes `userDetails` do usuário. 

| Atributo | Propriedade | Descrição |
| --- | --- | -- |
| user-details | userDetails | De definir o objeto do usuário que será exibido no controle. |

O exemplo a seguir define os detalhes da pessoa.

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

A `userDetails` `null` configuração para irá para o estado de saída.

Use os `loginInitiated` eventos e para manipular a saída e a `logoutInitiated` saída. 

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-login` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --weith: '100%';
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --button-color: #201f1e;
  --button-color--hover: var(--theme-primary-color);
  --button-background-color: transparent;
  --button-background-color--hover: #edebe9;
  --popup-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do controle.

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`loginInitiated` | O usuário clicou no botão entrar para iniciar o processo de logon | Nenhum | Sim | Não | Sim
`loginCompleted` | O processo de logon foi bem-sucedido e o usuário agora está login | Nenhum | Não | Não | Sim
`loginFailed` | O usuário cancelou o processo de logon ou não pôde entrar | Nenhum | Não | Não | Sim
`logoutInitiated` | O usuário começou a fazer logout | Nenhum | Sim | Não | Sim
`logoutCompleted` | O usuário saiu | Nenhum | Não | Não | Sim

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="templates"></a>Modelos

O `mgt-login` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos `<template>` `data-type` valores listados na tabela a seguir. 

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| signed-in-button-content | personDetails: objeto person, `personImage` : cadeia de caracteres de imagem da pessoa | O modelo usado para renderizar o conteúdo no botão quando o usuário está assinado. |
| signed-out-button-content | null | O modelo usado para renderizar o conteúdo no botão quando o usuário não estiver assinado. |
| comandos de sub- | handleSignOut: função de saída | O modelo usado para renderizar os comandos no flyout |
| flyout-person-details | personDetails: objeto person, personImage: cadeia de caracteres de imagem da pessoa | O modelo usado para renderizar os detalhes da pessoa no sobremenu. |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa as seguintes APIs Graph Microsoft e permissões:

| Configuração | Permissão | API
| - | - | - |
| Padrão. | User.Read | [/users/me/](/graph/api/user-get) |

Ao usar o padrão e os modelos, esse componente usa o componente Person para exibir o usuário e `signed-in-button-content` `flyout-person-details` herda todas as permissões. [](./person.md)

## <a name="authentication"></a>Autenticação

O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md). 

## <a name="cache"></a>Cache

Esse componente usa o [componente Person](./person.md) para exibir o usuário e herda toda a configuração de cache dele.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.

| Método | Descrição |
| - | - |
| renderButton | Renderiza o botão cromado. |
| renderButtonContent | Renderiza o conteúdo do botão. |
| renderSignedInButtonContent | Renderizar o conteúdo do botão quando o usuário estiver dentro. |
| renderSignedOutButtonContent | Renderizar o conteúdo do botão quando o usuário não estiver assinado. |
| renderFlyout | Renderiza o cromado do flyout. |
| renderFlyoutContent | Renderiza o conteúdo do sobrevoo. |
| renderFlyoutPersonDetails | Renderizar os detalhes da pessoa do sobrevoo. |
| renderFlyoutCommands | Renderizar os comandos de sobrevoo. |

### <a name="bring-your-own-flyout"></a>Traga seu próprio flyout

É possível usar seu próprio componente sub-1 no lugar do um integrado, substituindo o método e fornecendo `renderFlyout()` o novo sub-20.

Nesse caso, certifique-se de que o componente de logon continue a funcionar conforme o esperado substituindo os métodos de exibição do sobrevoo para atualizar a visibilidade do seu `protected` flyout alternativo.

| Método | Descrição |
| - | - |
| hideFlyout | Descarta o sobrevoo. |
| showFlyout | Exibe o sobrevoo. |
| toggleFlyout | Alterna o estado do sobrevoo. |
