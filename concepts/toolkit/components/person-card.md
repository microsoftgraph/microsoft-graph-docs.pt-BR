---
title: Person-Card componente no Kit de Ferramentas do Microsoft Graph
description: Um Person-Card componente é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: abee2c015c2dbaf53202b132c425a4a12df6ac30
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115224"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card componente no Kit de Ferramentas do Microsoft Graph

Um Person-Card componente é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Ele geralmente é usado como um flyout no `mgt-person` componente.

Para obter mais informações sobre `mgt-person` o componente, consulte [mgt-person](./person.md).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente. Passe o mouse sobre a pessoa para ver o [](#properties) Cartão de Pessoa e use o editor de código para ver como as propriedades alteram o comportamento do componente.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a>Configuração de componente global

A `MgtPersonCard` classe expõe um objeto `config` estático que configura todos os componentes de cartão de pessoa no aplicativo. O objeto config configura quais seções e quais APIs são usadas pelo cartão da pessoa para buscar detalhes sobre um usuário do Microsoft Graph.

Por padrão, todas as seções e APIs estão habilitadas. O exemplo a seguir mostra como usar o objeto config para desabilitar seções ou APIs.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

As propriedades a seguir estão disponíveis no objeto config.

| Propriedade | Descrição |
| ------------ | ------------- |
| useContactApis | `boolean` – Indica se o componente cartão de pessoa pode usar a API de Contato do Microsoft Graph para pesquisar detalhes e fotos do contato. O valor padrão é `true`.  |
| seções | `object` - Configura quais seções são mostradas no cartão da pessoa.  |

### <a name="person-card-sections"></a>Seções do cartão da pessoa

O cartão da pessoa contém várias seções configuráveis para exibir detalhes da pessoa:
* Contato - Informações de contato, como email, telefone, posição, local e muito mais.
* Organização – Gráfico organizacional com gerentes, relatórios diretos e pessoas relevantes.
* Mensagens - Mensagens de email mais relevantes com o usuário atualmente assinado.
* Arquivos - arquivos compartilhados mais relevantes com o usuário atualmente assinado.
* Perfil – informações de perfil, como projetos, habilidades, idiomas e muito mais.

As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio da `MgtPersonCard.config.sections` propriedade do objeto. As propriedades a seguir estão disponíveis.

| Propriedade | Descrição |
| ------------ | ------------- |
| organization | `boolean` - Indica se a seção da organização do cartão de pessoa é exibida. O valor padrão é `true`.  |
| mailMessages | `boolean` - Indica se a seção de mensagens do cartão da pessoa é exibida. O valor padrão é `true`.  |
| arquivos | `boolean` - Indica se a seção de arquivos de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| perfil | `boolean` - Indica se a seção de perfil de cartão de pessoa é mostrada. O valor padrão é `true`.  |

Para desabilitar uma seção, basta definir a propriedade como `false` no código de inicialização do aplicativo:
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Configuração para integrações do Teams

O Person-Card componente permite que o usuário entre em contato com a pessoa de destino, incluindo por meio de chat do Teams. Se estiver usando o componente dentro de um aplicativo de guia do Teams, você pode garantir que o componente se vincula diretamente a um chat em vez de abrir uma janela do navegador configurando o `microsoftTeamsLib` em `TeamsProvider` .

Se o Person-Card componente não puder detectar a biblioteca do Teams, o componente tentará abrir o cliente Web do Teams.

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

Para saber mais sobre o `TeamsProvider` provedor, confira [o provedor do Microsoft Teams.](../providers/teams.md)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-person` componente passará os detalhes da pessoa para o `mgt-person-card` componente. No entanto, você pode usar esses atributos para alterar isso ao modificar o componente ou ao usar o componente como `mgt-person` `mgt-person-card` um componente autônomo.

| Atributo         | Tipo                     | Descrição                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário. |
| person-image   | string                    | URI da imagem relacionada à pessoa exibida no cartão.                                   |
| inherit-details   | Nenhum.                  | Permite que o cartão de pessoa ande na árvore pai `mgt-person` do componente para usar o mesmo e os `person-details` `person-image` dados.                      |
| user-id | string | Permite que os desenvolvedores fornecem a ID de usuário para recuperar dados mostrados no componente person-card |
| person-query | string | Permite que os desenvolvedores fornecem consulta de pessoa para recuperar dados mostrados no componente person-card |


## <a name="templates"></a>Modelos

O Person-Card componente usa [modelos](../customize-components/templates.md) que permitem adicionar ou substituir partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir `<template>` o valor como um dos `data-type` seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| - | - | - |
| no-data | null | O modelo usado quando não há dados disponíveis.
| Padrão. | `person`: O objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo padrão substitui todo o componente pelo seu próprio. |
| person-details | `person`: O objeto de detalhes da pessoa | O modelo usado para renderizar a parte superior do cartão da pessoa. |
| additional-details | `person`: O objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo usado para adicionar conteúdo personalizado ao contêiner de detalhes adicionais. |

Por exemplo, você pode usar um modelo para personalizar o componente anexado ao componente e um modelo para adicionar `mgt-person` mais detalhes no cartão. 

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

## <a name="css-custom-properties"></a>Propriedades personalizadas css

O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS. 

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

Para saber mais, consulte [os componentes de estilo.](../customize-components/style.md)

## <a name="microsoft-graph-apis-and-permissions"></a>APIs e permissões do Microsoft Graph

O Person-Card controle usa as seguintes APIs e permissões do Microsoft Graph.

| Recurso | Permissão | Seção |
| - | - | - |
| [/me](/graph/api/user-get) | User.Read | Padrão |
| [/me/photo/$value](/graph/api/profilephoto-get) | User.Read | Padrão |
| [/me/people/?$search=](/graph/api/user-list-people) | People.Read | Padrão |
| [/me/contacts/\*](/graph/api/user-list-contacts) | Contacts.Read | Padrão |
| [/users/{id}](/graph/api/user-list-people) | User.ReadBasic.All | Padrão |
| [/users/{id}/photo/$value](/graph/api/profilephoto-get) | User.ReadBasic.All | Padrão |
| [/me/presence](/graph/api/presence-get) | Presence.Read | Padrão |
| [/users/{id}/presence](/graph/api/presence-get) | Presence.Read.All | Padrão |
| [/users/{id}/manager](/graph/api/user-list-manager) | User.Read.All | Organização |
| [/users/{id}/directReports](/graph/api/user-list-directreports) | User.Read.All | Organização |
| [/users/{id}/people](/graph/api/user-list-people) | People.Read.All | Organização |
| [/me/messages](/graph/api/user-list-messages) | Mail.ReadBasic | Mensagens |
| [/me/insights/shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used) | Sites.Read.All | Arquivos |
| [/users/{id}/profile](/graph/api/profile-get) | User.Read.All | Perfil |

A classe também expõe um método estático que retorna uma matriz de escopos necessários para que o cartão de pessoa funcione com base na configuração `MgtPersonCard` global do cartão de `getScopes` pessoa.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>Autenticação

O Person-Card controle usa o provedor de autenticação global descrito na documentação [de autenticação.](../providers/providers.md) 
