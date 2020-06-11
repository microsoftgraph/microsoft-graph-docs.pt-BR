---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e08e98a29ab454dca546d0fda34b8292ad97bf2d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681876"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Componente Person no Microsoft Graph Toolkit

O componente pessoa é usado para exibir uma pessoa ou contato usando a foto, o nome, o endereço de email ou qualquer outro detalhe de pessoa.

O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário. Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .

## <a name="example"></a>Exemplo

O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente. Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>Configurando os detalhes da pessoa

Você pode usar três propriedades para definir os detalhes da pessoa. Use apenas uma das seguintes propriedades por instância:

* Defina o `user-id` atributo ou a `userId` propriedade para buscar o usuário do Microsoft Graph usando sua ID.

* Definir o `person-query` atributo ou a `personQuery` propriedade para pesquisar o Microsoft Graph em uma determinada pessoa. Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa. Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.

* Defina o `person-presence` atributo ou a `personPresence` propriedade para adicionar um emblema de presença ao avatar manualmente.

* Defina o `avatar-size` atributo ou a `avatarSize` propriedade como `small` ou `large` para determinar o tamanho do Avatar. Isso ajuda a adicionar o [emblema de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar. Você precisará escolher as propriedades personalizadas de CSS correspondentes indicadas abaixo para personalizar ainda mais o tamanho do Avatar. Por padrão, o valor é definido como o `auto` qual decidirá automaticamente como renderizar a presença com base na `view` propriedade. Recomendamos usar `small` o se o seu avatar for menor do que o medianiz 32px por medianiz 32px. 

* Use o `person-details` atributo ou `personDetails` propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  Se nenhuma imagem for fornecida, uma será buscada (se disponível).

## <a name="properties"></a>Propriedades

Você pode usar várias propriedades para personalizar o componente.

| Atributo       | Propriedade       | Descrição                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| ID de usuário         | userId         | Defina como uma ID de usuário para buscar os detalhes e a imagem do usuário do Microsoft Graph.|
| pessoa – consulta    | personQuery    | Defina como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e busque os detalhes e a imagem da primeira pessoa.|
| pessoa-detalhes  | personDetails  | Defina como um objeto que represente uma pessoa. Funciona com o objeto dos recursos pessoas, usuários, contatos ou grupos. |
| pessoa-imagem    | personImage    | Defina a imagem a ser mostrada para a pessoa. |
| presença de pessoa | personPresence | Definir a presença para a pessoa. |
| FETCH-Image     | fetchImage     | Defina o sinalizador para buscar `personImage` automaticamente a partir do Microsoft Graph com base no `personDetails` objeto fornecido pelo usuário. |
| modo de exibição            | modo de exibição           | Definido para controlar como a pessoa é renderizada. O padrão é`avatar` <br /> `avatar`-Mostrar somente avatar <br /> `oneline`-Mostrar avatar e primeira linha ( `displayName` por padrão) <br /> `twolines`-Mostrar avatar e duas linhas de texto ( `displayName` e `mail` por padrão)|
| linha1-Propriedade  | line1Property  | Define a propriedade do personDetails a ser usado para a primeira linha do texto. O padrão é `displayName`.|
| Linha2-Propriedade  | line2Property  | Define a propriedade do personDetails a ser usado para a segunda linha de texto. O padrão é `mail`.|
| show-Presence   | a presença   | Definir sinalizador para exibir a presença de pessoa-o padrão é `false` .|
| show-Name       | Nome do mesmo       | **Preterido-uso `view` .**  Definir sinalizador para exibir o nome de exibição da pessoa-o padrão é `false` . |
| Mostrar-email      | Enviar email      | **Preterido-uso `view` .** Definir sinalizador para exibir o email da pessoa-o padrão é `false` .        |

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;
  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;
  --details-spacing: 12px;
}
```

Para saber mais, confira [estilos de componentes](../style.md).

## <a name="templates"></a>Modelos

O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:

| Tipo de dados | Contexto de dados | Descrição |
| --------- | ------------ | ----------- |
| carregando | Nenhuma | O modelo a ser renderizado enquanto o componente está em um estado laoding. |
| sem dados | Nenhuma | O modelo a ser renderizado quando nenhuma imagem de pessoa ou dados estiver disponível. | 
| Padrão. | Person: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente pelo seu. |
| cartão de pessoa | Person: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique. |

O exemplo a seguir define um modelo para o componente Person.

```html
<mgt-person>
  <template>
    <div data-if="personImage">
      <img src="{{personImage}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a>Cartão Pessoal

O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.

### <a name="add-the-control-to-the-html-page"></a>Adicionar o controle à página HTML
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Atributo    |  Propriedade     | Descrição                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| cartão de pessoa | personCardInteraction | Uma enumeração para determinar a ação do usuário necessária para ativar o painel ou o menu suspenso `hover` `click` . O valor padrão é`none` |


Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este controle usa as seguintes APIs e permissões do Microsoft Graph.

| Resource                                                                                                    | Permission     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [/me](/graph/api/user-get?view=graph-rest-1.0)                              | User.Read          |
| [$value/me/Photo/](/graph/api/profilephoto-get?view=graph-rest-beta)        | User.Read          |
| [/me/People/? $search =](/graph/api/user-list-people?view=graph-rest-1.0)     | People.Read        |
| [/me/contacts/\*](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | Contacts.Read      |
| [$value/Users/{ID}/Photo/](/graph/api/user-list-people?view=graph-rest-1.0) | User.ReadBasic.All |
| [/me/presence](/graph/api/presence-get?view=graph-rest-beta)                | Presence.Read |
| [/users/{id}/presence](/graph/api/presence-get?view=graph-rest-beta)        | Presence.Read.All |

> **Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza quando nenhum dado de imagem ou pessoa está disponível. |
| renderAvatar | Renderiza o Avatar. |
| renderDetails | Renderiza a parte de detalhes da pessoa. |
