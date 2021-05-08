---
title: Componente person no microsoft graph Toolkit
description: O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5250919404ecccea1f01042d93aaf2b9fa4fc3b3
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266840"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Componente person no microsoft graph Toolkit

O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome, endereço de email ou qualquer outro detalhe de pessoa.

O componente de pessoa também usa [o mgt-person-card](./person-card.md) para exibir um cartão de sub-sub-uso com informações adicionais sobre o usuário. Para obter detalhes, consulte a [seção Cartão de](#person-card) Pessoa.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>Definindo os detalhes da pessoa

Você pode usar três propriedades para definir os detalhes da pessoa. Use apenas uma das seguintes propriedades por instância:

* De definir `user-id` o atributo ou a propriedade para buscar o usuário do Microsoft Graph usando sua `userId` ID.

* De definir `person-query` o atributo ou a propriedade para pesquisar o Microsoft Graph por uma determinada `personQuery` pessoa. Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa. Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.

* De definir `person-presence` o atributo ou a propriedade para adicionar um selo de presença ao avatar da pessoa `personPresence` manualmente.

* De definir `avatar-size` o atributo ou a propriedade como ou para determinar o tamanho do `avatarSize` `small` `large` avatar. Isso ajuda a adicionar [o selo de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar. Você precisará escolher as propriedades personalizadas css correspondentes corretas mostradas abaixo para personalizar ainda mais o tamanho do avatar. Por padrão, o valor é definido para o qual decidirá automaticamente como renderizar a `auto` presença com base na `view` propriedade. Recomendamos usar `small` se seu avatar for menor que 32px por 32px. 

* Use o atributo ou a propriedade para definir manualmente os detalhes da `person-details` `personDetails` pessoa, conforme mostrado no exemplo a seguir.


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
| user-id         | userId         | De acordo com uma id do usuário para buscar os detalhes e a imagem desse usuário do Microsoft Graph.|
| person-query    | personQuery    | De definida como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e buscar os detalhes e a imagem da primeira pessoa.|
| person-details  | personDetails  | De acordo com um objeto que representa uma pessoa. Funciona com o objeto de pessoas, usuários, contatos ou grupos, recursos. |
| fallback-details| fallbackDetails| De acordo com um objeto que representa uma pessoa quando nenhum usuário/pessoa/contato é encontrado no gráfico.
| person-image    | personImage    | De definir a imagem para mostrar para a pessoa. |
| presença de pessoa | personPresence | Desmarcar a presença da pessoa. |
| fetch-image     | fetchImage     | De definir o sinalizador `personImage` para buscar automaticamente do Microsoft Graph com base `personDetails` no objeto fornecido pelo usuário. |
| tipo avatar     | avatarType     | Definir ou `initials` `photo` renderizar o estado de exibição - o padrão é foto. |
| modo de exibição            | modo de exibição           | Definir para controlar como a pessoa é renderizada. O padrão é `avatar` <br /> `avatar` - mostrar somente o avatar <br /> `oneline` - mostrar avatar e primeira linha ( `displayName` por padrão) <br /> `twolines` - mostrar avatar e duas linhas de texto ( `displayName` `mail` e por padrão)|
| line1-property  | line1Property  | Define a propriedade da personDetails a ser usada para a primeira linha de texto. O padrão é `displayName`.|
| line2-property  | line2Property  | Define a propriedade da personDetails a ser usada para a segunda linha de texto. O padrão é `mail`.|
| line3-property  | line3Property  | Define a propriedade da personDetails a ser usada para a terceira linha de texto. O padrão é `jobTitle`.|
| show-presence   | showPresence   | Definir sinalizador para exibir a presença da pessoa - o padrão é `false` .|

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-person` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  
  --initials-color: white;
  --initials-background-color: magenta;

  --presence-background-color: #ffffff;
  --presence-icon-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: black;
  --line3-text-transform: none;

  --details-spacing: 12px;
}
```

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

| Evento | Detalhe | Descrição |
| --- | --- | --- |
| line1clicked | O detalhe contém o objeto `person` respectivo | Acionado quando a linha1 é clicada. |
| line2clicked | O detalhe contém o objeto `person` respectivo | Disparado quando a linha2 é clicada. |
| line3clicked | O detalhe contém o objeto `person` respectivo | Acionado quando a linha3 é clicada. |

## <a name="templates"></a>Modelos

O `mgt-person` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:

| Tipo de dados | Contexto de dados | Descrição |
| --------- | ------------ | ----------- |
| loading | nenhuma | O modelo a ser render enquanto o componente está em um estado de carregamento. |
| no-data | nenhuma | O modelo a ser renderizar quando nenhuma imagem ou dados de pessoa estiver disponível. | 
| Padrão. | pessoa: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente por seu próprio. |
| person-card | pessoa: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo para atualizar o mgt-person-card exibido em foco ou clique. |
| line1 | pessoa: o objeto de detalhes da pessoa | O modelo para a primeira linha de metadados de pessoa. |
| line2 | pessoa: o objeto de detalhes da pessoa | O modelo para a segunda linha de metadados de pessoa. |
| line3 | pessoa: o objeto de detalhes da pessoa | O modelo para a terceira linha de metadados de pessoa. |

O exemplo a seguir define um modelo para o componente da pessoa.

```html
<!-- Retemplate the entire person component -->
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

<!-- Retemplate the line properties -->
<mgt-person view="threeLines">
  <template data-type="line1">
    <div>
      Hello, my name is: {{person.displayName}}
    </div>
  </template>
  <template data-type="line2">
    <div>
      Super cool
    </div>
  </template>
  <template data-type="line3">
    <div>
      Loves MGT
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a>Cartão pessoal

O `mgt-person` componente pode mostrar um ao passar o mouse ou `mgt-person-card` clicar.

### <a name="add-the-control-to-the-html-page"></a>Adicionar o controle à página HTML
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Atributo    |  Propriedade     | Descrição                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover` ou `click` . O valor padrão é `none` |


Para obter mais informações sobre a templating, o estilo e os atributos, consulte [Person Card component](./person-card.md).

## <a name="global-component-configuration"></a>Configuração de componente global

A `MgtPerson` classe expõe um objeto `config` estático que configura todos os componentes da pessoa no aplicativo.

O exemplo a seguir mostra como usar o objeto config.

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

As propriedades a seguir estão disponíveis no objeto config.

| Propriedade | Descrição |
| ------------ | ------------- |
| useContactApis | `boolean` - Indica se o componente da pessoa pode usar a API de contatos pessoais do Microsoft Graph para pesquisar detalhes de contato e fotos. O valor padrão é `true`.  |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Esse controle usa as seguintes APIs e permissões do Microsoft Graph.

| Recurso | Permissão     |
| -| - |
| [/me](/graph/api/user-get)                              | User.Read          |
| [/me/photo/$value](/graph/api/profilephoto-get)        | User.Read          |
| [/me/people/?$search=](/graph/api/user-list-people)     | People.Read        |
| [/me/contacts/\*](/graph/api/user-list-contacts&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](/graph/api/user-list-people) | User.ReadBasic.All |
| [/me/presence](/graph/api/presence-get)                | Presence.Read |
| [/users/{id}/presence](/graph/api/presence-get)        | Presence.Read.All |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`photos`|Foto da pessoa|Usado, quando `avatarType` é definido como e é definido `photo` `fetchImage` como `true`|
|`presence`|Presença da pessoa|Usado, quando `showPresence` está definido como `true`|
|`users`|Informações do usuário da pessoa|

Consulte [Cache para](../customize-components/cache.md) obter mais detalhes sobre como configurar o cache.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza quando nenhum dado de imagem ou pessoa está disponível. |
| renderAvatar | Renderiza o avatar. |
| renderDetails | Renderiza a parte de detalhes da pessoa. |
