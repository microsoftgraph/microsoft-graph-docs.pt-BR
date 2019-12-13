---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ab9dc1bef81585bb71cdb29de015d8adb6030110
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955852"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Componente Person no Microsoft Graph Toolkit

O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email. 

O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário. Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .

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

Você pode usar várias propriedades para personalizar o componente.

| Atributo    | Propriedade   | Descrição                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| show-Name    | Nome do mesmo   | Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é. |
| Mostrar-email   | Enviar email  | Definir sinalizador para exibir o email da pessoa- `false`o padrão é.        |

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

| Tipo de dados     | Contexto de dados              | Descrição                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| Padrão.     | Person: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente pelo seu. |
| cartão de pessoa | Person: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique. |

O exemplo a seguir define um modelo para o componente Person.

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

## <a name="person-card"></a>Cartão de pessoa

O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.

### <a name="add-the-control-to-the-html-page"></a>Adicionar o controle à página HTML
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Atributo    |  Propriedade     | Descrição                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| cartão de pessoa | personCard | Uma enumeração para determinar a ação do usuário necessária para ativar o `hover` painel `click`ou o menu suspenso. O valor padrão é`none` |


Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este controle usa as seguintes APIs e permissões do Microsoft Graph.

| Resource                                                                                                    | Permissão     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [/me](https://docs.microsoft.com/graph/api/user-get?view=graph-rest-1.0)                              | User.Read          |
| [$value/me/Photo/](https://docs.microsoft.com/graph/api/profilephoto-get?view=graph-rest-beta)        | User.Read          |
| [/me/People/? $search =](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0)     | People.Read        |
| [/me/contacts/*](https://docs.microsoft.com/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | Contacts.Read      |
| [$value/Users/{ID}/Photo/](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0) | User.ReadBasic.All |

> **Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.
