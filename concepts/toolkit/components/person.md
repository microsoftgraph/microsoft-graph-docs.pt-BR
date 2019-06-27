---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9102259258bb691dee2c56449257740db7b1913
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242926"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Componente Person no Microsoft Graph Toolkit

O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email. 

## <a name="example"></a>Exemplo

[exemplo de jsfiddle](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a>Adicionar o controle à página HTML
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a>Configurando os detalhes da pessoa

Você pode usar três propriedades para definir os detalhes da pessoa. Use apenas uma das seguintes propriedades por instância:

* Defina o `user-id` atributo ou `userId` a propriedade para buscar o usuário do Microsoft Graph usando sua ID.  

* Definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph em uma determinada pessoa. Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa. Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.

* Defina o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  Se nenhuma imagem for fornecida, uma será buscada (se disponível).

## <a name="changing-how-the-component-looks"></a>Alterar a aparência do componente

Você pode usar várias Propriedadespara personalizar o componente.

| Propriedade | Atributo | Descrição |
| --- | --- | --- |
| `showName` | `show-name` | Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é. |
| `showEmail` | `show-email` | Definir sinalizador para exibir o email da pessoa- `false`o padrão é. |

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

Para saber mais, confira [estilos de componentes](../style.md).

## <a name="templates"></a>Modelos

O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| `default` | `person`: um objeto Person | O modelo padrão substitui todo o componente pelo seu. |

O exemplo a seguir define um modelo para o componente Person:

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este controle usa as seguintes APIs e permissões do Microsoft Graph.

| Resource | Permissão/escopo |
| - | - |
| [/me](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0) | `User.Read` |
| [$value/me/Photo/](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta) | `User.Read` |
| [/me/People/? $search =](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |
| [/me/contacts/*](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | `Contacts.Read` |
| [$value/Users/{ID}/Photo/](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `User.ReadBasic.All` |

> **Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.
