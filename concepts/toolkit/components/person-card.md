---
title: Person-Card componente no microsoft Graph Toolkit
description: Um Person-Card é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 58efcb2c1ca7ec1e366340b1dcbe199fe054c7b8
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334749"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card componente no microsoft Graph Toolkit

Um Person-Card é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Geralmente, ele é usado como um sobrevoo no `mgt-person` componente.

Para obter mais informações sobre o `mgt-person` componente, consulte [mgt-person](./person.md).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente. Passe o mouse sobre a pessoa para ver o [](#properties) Cartão de Pessoa e use o editor de código para ver como as propriedades alteram o comportamento do componente.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a>Configuração de componente global

A `MgtPersonCard` classe expõe um objeto `config` estático que configura todos os componentes de cartão de pessoa no aplicativo. O objeto config configura quais seções e quais APIs são usadas pelo cartão de pessoa para buscar detalhes sobre um usuário do Microsoft Graph.

Por padrão, todas as seções e APIs estão habilitadas. O exemplo a seguir mostra como usar o objeto config para desabilitar seções ou APIs.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

As propriedades a seguir estão disponíveis no objeto config.

| Propriedade | Descrição |
| ------------ | ------------- |
| useContactApis | `boolean`- Indica se o componente de cartão de pessoa pode usar a API de contato do Microsoft Graph para pesquisar detalhes e fotos de contato. O valor padrão é `true`.  |
| seções | `object` - Configura quais seções são mostradas no cartão de pessoa.  |

### <a name="person-card-sections"></a>Seções de cartão de pessoa

O cartão de pessoa contém várias seções configuráveis para exibir detalhes da pessoa:
* Contato - Informações de contato como email, telefone, posição, local e muito mais.
* Organização - Gráfico organizacional com gerentes, relatórios diretos e pessoas relevantes.
* Mensagens - Mensagens de email mais relevantes com o usuário atualmente assinado.
* Arquivos - Arquivos compartilhados mais relevantes com o usuário atualmente assinado.
* Perfil - Informações de perfil, como projetos, habilidades, idiomas e muito mais.

As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio `MgtPersonCard.config.sections` da propriedade object. As propriedades a seguir estão disponíveis.

| Propriedade | Descrição |
| ------------ | ------------- |
| organization | `boolean` - Indica se a seção organização do cartão de pessoa é mostrada. O valor padrão é `true`.  |
| mailMessages | `boolean` - Indica se a seção mensagens de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| arquivos | `boolean` - Indica se a seção arquivos de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| perfil | `boolean` - Indica se a seção perfil de cartão de pessoa é mostrada. O valor padrão é `true`.  |

Para desabilitar uma seção, basta definir a propriedade como `false` no código de inicialização do aplicativo:
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Instalação para Teams integrações

O Person-Card componente permite que o usuário entre em contato com a pessoa de destino, incluindo Teams chat. Se usar o componente dentro de um aplicativo de guia Teams, você pode garantir que o componente se vincula diretamente a um chat em vez de abrir uma janela do navegador definindo o `microsoftTeamsLib` em `TeamsProvider` .

Se o Person-Card não puder detectar a Teams, o componente tentará abrir o cliente Teams Web.

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

Para obter mais informações sobre o `TeamsProvider` provedor, [consulte Microsoft Teams provedor](../providers/teams.md).

## <a name="properties"></a>Propriedades

Por padrão, `mgt-person` o componente passará os detalhes da pessoa para o `mgt-person-card` componente. No entanto, você pode usar esses atributos para alterar isso ao tentar emplacar o componente ou ao usar o componente `mgt-person` `mgt-person-card` como um componente autônomo.

| Atributo         | Tipo                     | Descrição                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário. |
| person-image   | string                    | Uri de imagem relacionado à pessoa exibida no cartão.                                   |
| inherit-details   | Nenhum.                  | Permite que o cartão de pessoa ande na árvore pai para `mgt-person` que o componente use os mesmos e os `person-details` `person-image` dados.                      |
| user-id | string | Permite que os desenvolvedores fornecem a ID do usuário para recuperar dados mostrados no componente person-card |
| person-query | string | Permite que os desenvolvedores fornecem consulta de pessoa para recuperar dados mostrados no componente person-card |


## <a name="templates"></a>Modelos

O Person-Card componente usa [modelos](../customize-components/templates.md) que permitem adicionar ou substituir partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| - | - | - |
| no-data | null | O modelo usado quando nenhum dado está disponível.
| Padrão. | `person`: O objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente por seu próprio. |
| person-details | `person`: O objeto de detalhes da pessoa | O modelo usado para renderizar a parte superior do cartão de pessoa. |
| detalhes adicionais | `person`: O objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo usado para adicionar conteúdo personalizado ao contêiner de detalhes adicionais. |

Por exemplo, você pode usar um modelo para personalizar o componente anexado ao componente e um modelo para adicionar `mgt-person` detalhes adicionais no cartão. 

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

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`expanded` | O usuário abriu a seção detalhes expandidos do cartão | Nenhum | Não | Sim | Sim, a menos que você substitua o modelo padrão

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-person-card` componente define as seguintes propriedades personalizadas CSS. 

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
}
```

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

O controle Person-Card usa as seguintes APIs Graph Microsoft e permissões.

| Configuração | Permissão | API | Section |
| --- | ---------- | ------- | --------- |
| `personDetails` set with user's `id` but without e-mail, or `userId` set, or set `personQuery` to `me` | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get) | Padrão |
| `personQuery` definido como um valor diferente do `me` | People.Read | [/me/people/?$search=](/graph/api/user-list-people) | Padrão |
| `personQuery` definido como um valor diferente `me` e `config.useContactApis` definido como `true` (padrão) | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) | Padrão |
| `showPresence` set to `true` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) | Padrão |
| `sections.organization` habilitado (padrão) | User.Read.All | [/users/{id}/manager](/graph/api/user-list-manager) | Organização |
| `sections.organization.showWorksWith` set (padrão) | People.Read.All | [/users/{id}/people](/graph/api/user-list-people) | Organização |
| `sections.mailMessages` habilitado (padrão) | Mail.ReadBasic | [/me/messages](/graph/api/user-list-messages) | Mensagens |
| `sections.files` habilitado (padrão) | Sites.Read.All | [/me/insights/shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used) | Arquivos |

A classe também expõe um método estático que retorna uma matriz de escopos necessários para que o cartão de pessoa funcione com base na configuração `MgtPersonCard` global do cartão de `getScopes` pessoa.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>Autenticação

O Person-Card usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md). 

## <a name="cache"></a>Cache

> [!IMPORTANT]
> O `mgt-person-card` componente recupera os dados básicos da pessoa do componente pai sem chamar o Microsoft `mgt-person` Graph. Quando `mgt-person-card` for usado separadamente, ele recuperará os dados necessários em si e os armazenará em cache. Os dados exibidos nas seções do cartão são recuperados separadamente e não são armazenados em cache.

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`people`|Informações da pessoa|Usado quando `personQuery` especificado e seu valor é diferente do `me`|
|`photos`|Foto da pessoa|
|`presence`|Presença da pessoa|Usado, quando `showPresence` está definido como `true`|
|`users`|Informações do usuário da pessoa|Usado quando `userId` especificado ou `personQuery` definido como `me`|

Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.
