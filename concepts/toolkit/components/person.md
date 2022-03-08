---
title: Componente person no microsoft Graph Toolkit
description: O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: 59f2c6f286aa176ea2ebdad0044388bcfb25f896
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336106"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Componente person no microsoft Graph Toolkit

O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome, endereço de email ou qualquer outro detalhe de pessoa.

O componente de pessoa também usa [o mgt-person-card](./person-card.md) para exibir um cartão de sub-sub-uso com informações adicionais sobre o usuário. Para obter detalhes, consulte a [seção Cartão de](#person-card) Pessoa.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>Definindo os detalhes da pessoa

Você pode usar três propriedades para definir os detalhes da pessoa. Use apenas uma das seguintes propriedades por instância:

* De definir o `user-id` atributo ou `userId` a propriedade para buscar o usuário da Microsoft Graph usando sua ID.

* De definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph uma determinada pessoa. Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa. Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.

* De definir o `person-presence` atributo ou `personPresence` a propriedade para adicionar um selo de presença ao avatar da pessoa manualmente.

* De definir o `avatar-size` atributo ou `avatarSize` a propriedade como `small` ou `large` para determinar o tamanho do avatar. Isso ajuda a adicionar [o selo de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar. Você precisará escolher as propriedades personalizadas css correspondentes corretas mostradas abaixo para personalizar ainda mais o tamanho do avatar. Por padrão, o valor é definido para `auto` o qual decidirá automaticamente como renderizar a presença com base na `view` propriedade. Recomendamos usar `small` se seu avatar for menor que 32px por 32px. 

* Use o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  Se nenhuma imagem for fornecida, uma será buscada (se disponível).

* Por padrão, o componente de pessoa solicitará apenas o conjunto de propriedades padrão da Microsoft Graph [usuário.](/graph/api/user-get?&tabs=http#optional-query-parameters) Para solicitar propriedades adicionais, declare-as como qualquer parte do `line(x)Property`. 


## <a name="properties"></a>Propriedades

Você pode usar várias propriedades para personalizar o componente.

| Atributo       | Propriedade       | Descrição                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| user-id         | userId         | De acordo com uma id do usuário para buscar os detalhes e a imagem desse usuário da Microsoft Graph.|
| person-query    | personQuery    | De definida como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e buscar os detalhes e a imagem da primeira pessoa.|
| person-details  | personDetails  | De acordo com um objeto que representa uma pessoa. Funciona com o objeto de pessoas, usuários, contatos ou grupos, recursos. |
| fallback-details| fallbackDetails| De acordo com um objeto que representa uma pessoa quando nenhum usuário/pessoa/contato é encontrado no gráfico.
| person-image    | personImage    | De definir a imagem para mostrar para a pessoa. |
| presença de pessoa | personPresence | Desmarcar a presença da pessoa. |
| fetch-image     | fetchImage     | De definir o sinalizador para buscar `personImage` automaticamente do Microsoft Graph com base no `personDetails` objeto fornecido pelo usuário. |
| disable-image-fetch | disableImageFetch | De definir sinalizador para desabilitar a busca da imagem da pessoa. Pode ser usado para evitar busca desnecessária da Microsoft Graph ao especificar a `personImage` propriedade.
| tipo avatar     | avatarType     | Definir ou `initials` renderizar `photo` o estado de exibição - o padrão é foto. |
| modo de exibição            | modo de exibição           | Definir para controlar como a pessoa é renderizada. O padrão é `avatar` <br /> `avatar` - mostrar somente o avatar <br /> `oneline` - mostrar avatar e primeira linha (`displayName` por padrão) <br /> `twolines` - mostrar avatar e duas linhas de texto (`displayName` e `mail` por padrão) <br /> `threelines`- mostrar avatar e três linhas de texto (`displayName`e `jobTitle` por `mail` padrão) |
| line1-property  | line1Property  | Define a propriedade da personDetails a ser usada para a primeira linha de texto. O padrão é `displayName`.|
| line2-property  | line2Property  | Define a propriedade da personDetails a ser usada para a segunda linha de texto. O padrão é `mail`.|
| line3-property  | line3Property  | Define a propriedade da personDetails a ser usada para a terceira linha de texto. O padrão é `jobTitle`.|
| show-presence   | showPresence   | Definir sinalizador para exibir a presença da pessoa - o padrão é `false`.|

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-person` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --avatar-cursor: default;
  
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

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`line1clicked` | Disparado quando a linha1 é clicada | O `person` objeto que pode ser um usuário [Graph, pessoa](/graph/api/resources/user) ou [](/graph/api/resources/person) contato com [](/graph/api/resources/contact) uma propriedade adicional que contém a `personImage` URL da foto do usuário | Não | Não | Sim, a menos que você substitua o modelo padrão
`line2clicked` | Disparado quando a linha2 é clicada | O `person` objeto que pode ser um usuário [Graph, pessoa](/graph/api/resources/user) ou [](/graph/api/resources/person) contato com [](/graph/api/resources/contact) uma propriedade adicional que contém a `personImage` URL da foto do usuário | Não | Não | Sim, a menos que você substitua o modelo padrão
`line3clicked` | Disparado quando a linha3 é clicada | O `person` objeto que pode ser um usuário [Graph, pessoa](/graph/api/resources/user) ou [](/graph/api/resources/person) contato com [](/graph/api/resources/contact) uma propriedade adicional que contém a `personImage` URL da foto do usuário | Não | Não | Sim, a menos que você substitua o modelo padrão

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="templates"></a>Modelos

O `mgt-person` componente dá suporte a [vários modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes:

| Tipo de dados | Contexto de dados | Descrição |
| --------- | ------------ | ----------- |
| loading | none | O modelo a ser render enquanto o componente está em um estado de carregamento. |
| no-data | none | O modelo a ser renderizar quando nenhuma imagem ou dados de pessoa estiver disponível. | 
| Padrão. | pessoa: o objeto de detalhes da pessoa <br> `personImage`: A URL da imagem <br> `personPresence`: O objeto de detalhes de presença para pessoa  | O modelo padrão substitui todo o componente por seu próprio. |
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

O `mgt-person` componente pode mostrar um `mgt-person-card` ao passar o mouse ou clicar.

### <a name="add-the-control-to-the-html-page"></a>Adicionar o controle à página HTML
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| Atributo    |  Propriedade     | Descrição                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover` ou `click`. O valor padrão é `none` |


Para obter mais informações sobre a templating, o estilo e os atributos, consulte [Person Card component](./person-card.md).

## <a name="global-component-configuration"></a>Configuração de componente global

A `MgtPerson` classe expõe um objeto estático `config` que configura todos os componentes da pessoa no aplicativo.

O exemplo a seguir mostra como usar o objeto config.

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

As propriedades a seguir estão disponíveis no objeto config.

| Propriedade | Descrição |
| ------------ | ------------- |
| useContactApis | `boolean`- Indica se o componente da pessoa pode usar a API de contatos pessoais da Microsoft Graph para pesquisar detalhes de contato e fotos. O valor padrão é `true`.  |

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Esse controle usa as seguintes APIs Graph Microsoft e permissões.

| Configuração | Permissão | API |
| ------------- | ---------- | --- |
| `personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo`, retrieved person is a contact and `useContactApis` set to `true` | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) |
| `personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and person is not a contact or `useContactApis` is set to `false` | User.ReadBasic.All | [/users/{id}/photo/$value](/graph/api/profilephoto-get) |
| `personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and user specified via email | User.ReadBasic.All | [/users/{id}/photo/$value](/graph/api/profilephoto-get) |
| `personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to and `photo` contact specified via email | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) |
| `userId` set | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people) |
| `personQuery` definir como `me` e `avatarType` definir como `photo` | User.Read | [/me/photo/$value](/graph/api/profilephoto-get) |
| `personQuery` definir para `me` e `avatarType` definir para outra coisa que não `photo` | User.Read | [/me](/graph/api/user-get) |
| `personQuery` definido como um valor diferente e `me` `useContactApis` definido como `true` | People.Read, User.ReadBasic.All, Contacts.Read | [/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/\*](/graph/api/user-list-contacts) |
| `personQuery` definido como um valor diferente e `me` `useContactApis` definido como `false` | People.Read, User.ReadBasic.All | [/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people) |
| `showPresence` definir como `true` e `personQuery` definir como `me` | Presence.Read | [/me/presence](/graph/api/presence-get) |
| `showPresence` definir como `true` e `personQuery` definir como um valor diferente `me` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) |
| `personCardInteraction` definido como um valor diferente de `PersonCardInteraction.none` | Consulte [permissões de cartão de pessoa](/graph/toolkit/components/person-card#microsoft-graph-permissions) | Consulte [chamadas de API de cartão de pessoa](/graph/toolkit/components/person-card#microsoft-graph-permissions) |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`photos`|Foto da pessoa|Usado, quando `avatarType` é definido como `photo` e `fetchImage` é definido como `true`|
|`presence`|Presença da pessoa|Usado, quando `showPresence` está definido como `true`|
|`users`|Informações do usuário da pessoa|

Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, `protected render*` esse componente expõe vários métodos para substituição em extensões de componentes.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza quando nenhum dado de imagem ou pessoa está disponível. |
| renderAvatar | Renderiza o avatar. |
| renderDetails | Renderiza a parte de detalhes da pessoa. |
