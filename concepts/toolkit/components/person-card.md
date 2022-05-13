---
title: Person-Card componente no Microsoft Graph Toolkit
description: Um Person-Card componente é um componente para exibir mais informações relacionadas a uma pessoa.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 20f34becb875b7bd8dd10bfdafce28fd6d14c808
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398318"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card componente no Microsoft Graph Toolkit

Um Person-Card componente é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Geralmente, ele é usado como um submenu no `mgt-person` componente.

Para obter mais informações sobre o `mgt-person` componente, consulte [mgt-person](./person.md).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do componente `mgt-person-card` com um `mgt-person` componente. Passe o mouse sobre a pessoa para ver o Cartão de Pessoa e use o editor de código para ver como as [propriedades alteram](#properties) o comportamento do componente.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a>Configuração de componente global

A `MgtPersonCard` classe expõe um objeto estático `config` que configura todos os componentes de cartão de pessoa no aplicativo. O objeto de configuração configura quais seções e quais APIs são usadas pelo cartão de pessoa para buscar detalhes sobre um usuário do Microsoft Graph.

Por padrão, todas as seções e APIs estão habilitadas. O exemplo a seguir mostra como usar o objeto de configuração para desabilitar seções ou APIs.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

As propriedades a seguir estão disponíveis no objeto de configuração.

| Propriedade | Descrição |
| ------------ | ------------- |
| useContactApis | `boolean`– Indica se o componente de cartão de pessoa pode usar a API de Contato do Microsoft Graph para pesquisar detalhes de contato e fotos. O valor padrão é `true`.  |
| seções | `object` – Configura quais seções são mostradas no cartão da pessoa.  |

### <a name="person-card-sections"></a>Seções de cartão de pessoa

O cartão de pessoa contém várias seções configuráveis para exibir detalhes da pessoa:
* Contato – Informações de contato, como email, telefone, posição, local e muito mais.
* Organização – Grafo organizacional com gerentes, relatórios diretos e pessoas relevantes.
* Mensagens – mensagens de email mais relevantes com o usuário conectado atual.
* Arquivos – Arquivos compartilhados mais relevantes com o usuário conectado atual.
* Perfil – Informações de perfil, como projetos, habilidades, idiomas e muito mais.

As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio da propriedade `MgtPersonCard.config.sections` de objeto. As propriedades a seguir estão disponíveis.

| Propriedade | Descrição |
| ------------ | ------------- |
| organization | `boolean` – Indica se a seção da organização do cartão de pessoa é mostrada. O valor padrão é `true`.  |
| mailMessages | `boolean` – Indica se a seção mensagens de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| arquivos | `boolean` – Indica se a seção de arquivos de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| perfil | `boolean` – Indica se a seção de perfil de cartão de pessoa é mostrada. O valor padrão é `true`.  |

Para desabilitar uma seção, basta definir a propriedade como `false` no código de inicialização do aplicativo:
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Configuração para Teams integrações

O Person-Card componente permite que o usuário entre em contato com a pessoa de destino, incluindo por meio Teams chat. Se estiver usando o componente dentro de um aplicativo de guia Teams, você poderá garantir que o componente seja vinculado diretamente a um chat `microsoftTeamsLib` em vez de abrir uma janela do navegador definindo a opção em `TeamsProvider`.

Se o Person-Card não puder detectar a biblioteca Teams, o componente tentará abrir o Teams web.

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

Para obter mais informações sobre o `TeamsProvider` provedor, [consulte Microsoft Teams provedor](../providers/teams.md).

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-person` componente passará os detalhes da pessoa para o `mgt-person-card` componente. No entanto, você pode usar esses atributos para alterar isso ao modelar `mgt-person` `mgt-person-card` o componente ou ao usar o componente como um componente autônomo.

| Atributo         | Tipo                     | Descrição                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| detalhes da pessoa | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Objeto person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário. |
| person-image   | string                    | URI de imagem relacionado à pessoa exibida no cartão.                                   |
| inherit-details   | Nenhum.                  | Permite que o cartão de pessoa ande na árvore pai para que `mgt-person` o componente use os mesmos dados `person-details` `person-image` .                      |
| id do usuário | cadeia de caracteres | Permite que os desenvolvedores forneçam a ID de usuário para recuperar os dados mostrados no componente cartão de pessoa |
| consulta de pessoa | string | Permite que os desenvolvedores forneçam consulta de pessoa para recuperar dados mostrados no componente cartão de pessoa |
| cartão de pessoa | string | Especifica que o componente `person-card` pode ser mostrado como um cartão pop-up quando você passa o mouse ou clica no `mgt-person` componente. Os valores permitidos são `hover` ou `click`.


## <a name="templates"></a>Modelos

O Person-Card componente usa [modelos que](../customize-components/templates.md) permitem adicionar ou substituir partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| - | - | - |
| sem dados | null | O modelo usado quando nenhum dado está disponível.
| Padrão. | `person`: o objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo padrão substitui todo o componente pelo seu próprio. |
| detalhes da pessoa | `person`: o objeto de detalhes da pessoa | O modelo usado para renderizar a parte superior do cartão de pessoa. |
| detalhes adicionais | `person`: o objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo usado para adicionar conteúdo personalizado ao contêiner de detalhes adicionais. |

Por exemplo, você pode usar um modelo para `mgt-person` personalizar o componente anexado ao componente e um modelo para adicionar detalhes adicionais no cartão. 

```html
    <mgt-person person-query="me" view="twolines" person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

Evento | Quando ele é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`expanded` | O usuário abriu a seção de detalhes expandida do cartão | Nenhum | Não | Sim | Sim, a menos que você substitua o modelo padrão

Para obter mais informações sobre como manipular eventos, consulte [eventos](../customize-components/events.md).

## <a name="css-custom-properties"></a>Propriedades personalizadas css

O `mgt-person-card` componente define as seguintes propriedades personalizadas css. 

```css
mgt-person {
  --person-card-display-name-font-size: 40px;
  --person-card-display-name-color: #ffffff;
  --person-card-title-font-size: 20px;
  --person-card-title-color: #ffffff;
  --person-card-subtitle-font-size: 10px;
  --person-card-subtitle-color: #ffffff;
  --person-card-details-title-font-size: 10px;
  --person-card-details-title-color: #b3bf0a;
  --person-card-details-item-font-size: 20px;
  --person-card-details-item-color: #3abf0a;
  --person-card-background-color: #000000;
  --person-card-contact-link-color: #ff0000;
  --person-card-contact-link-hover-color: #00ff00;
  --person-card-show-more-color: #ff0000;
  --person-card-show-more-hover-color: #00ff00;
  --person-card-base-links-color: #ff0000;
  --person-card-base-links-hover-color: #00ff00;
  --person-card-tab-nav-color: #ff0000;
  --person-card-active-org-member-color: #ff0000;
  --person-card-nav-back-arrow-hover-color: #00ff00;
  --person-card-nav-back-arrow-color: #ff0000;
}
```

Para saber mais, confira [os componentes de estilo](../customize-components/style.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

O Person-Card usa as seguintes APIs e permissões do Microsoft Graph.

| Configuração | Permissão | API | Section |
| --- | ---------- | ------- | --------- |
| `personDetails` definido com o usuário, `id` mas sem email, ou `userId` definido ou `personQuery` definido como `me` | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get) | Padrão |
| `personQuery` definido como um valor diferente de `me` | People.Read | [/me/people/?$search=](/graph/api/user-list-people) | Padrão |
| `personQuery` definido como um valor diferente e `me` definido `config.useContactApis` como `true` (padrão) | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) | Padrão |
| `showPresence` definido como `true` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) | Padrão |
| `sections.organization` habilitado (padrão) | User.Read.All | [/users/{id}/manager](/graph/api/user-list-manager) | Organização |
| `sections.organization.showWorksWith` set (padrão) | People.Read.All | [/users/{id}/people](/graph/api/user-list-people) | Organização |
| `sections.mailMessages` habilitado (padrão) | Mail.ReadBasic | [/me/messages](/graph/api/user-list-messages) | Mensagens |
| `sections.files` habilitado (padrão) | Sites.Read.All | [/me/insights/shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used) | Arquivos |
| `sections.profile` habilitado (padrão) | User.Read.All | [/users/{id}/profile](/graph/api/profile-get?view=graph-rest-beta&preserve-view=true) | Perfil |

A `MgtPersonCard` classe também expõe um `getScopes` método estático que retorna uma matriz de escopos necessários para que o cartão de pessoa funcione com base na configuração global do cartão de pessoa.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>Autenticação

O Person-Card usa o provedor de autenticação global descrito na documentação [de autenticação](../providers/providers.md). 

## <a name="cache"></a>Cache

> [!IMPORTANT]
> O `mgt-person-card` componente recupera os dados básicos da pessoa do componente pai `mgt-person` sem chamar o Microsoft Graph. Quando `mgt-person-card` for usado separadamente, ele recuperará os dados necessários em si e os armazenará em cache. Os dados exibidos nas seções do cartão são recuperados separadamente e não são armazenados em cache.

|Repositório de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`people`|Informações da pessoa|Usado quando `personQuery` é especificado e seu valor é diferente de `me`|
|`photos`|Foto da pessoa|
|`presence`|Presença da pessoa|Usado, quando `showPresence` é definido como `true`|
|`users`|Informações do usuário da pessoa|Usado quando `userId` é especificado ou é `personQuery` definido como `me`|

Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.
