---
title: Person-Card componente no kit de ferramentas do Microsoft Graph
description: Um componente de Person-Card é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 79a14c3d37fba06a076e319b34029008b7fbf2fd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659180"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card componente no kit de ferramentas do Microsoft Graph

Um componente de Person-Card é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Geralmente, é usado como um submenu do `mgt-person` componente.

Para obter mais informações sobre o `mgt-person` componente, consulte [Gerenciamento-pessoa](./person.md).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente. Passe o mouse sobre a pessoa para ver o cartão Person e use o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a>Configuração de componente global

A `MgtPersonCard` classe expõe um `config` objeto estático que configura todos os componentes de cartão de pessoa no aplicativo. O objeto config Configura quais seções e quais APIs são usadas pelo cartão de pessoa para buscar detalhes sobre um usuário do Microsoft Graph.

Por padrão, todas as seções e APIs estão habilitadas. O exemplo a seguir mostra como usar o objeto config para desabilitar seções ou APIs.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

As propriedades a seguir estão disponíveis no objeto config.

| Propriedade | Descrição |
| ------------ | ------------- |
| useContactApis | `boolean` – Indica se o componente de cartão de pessoa pode usar a API de contato do Microsoft Graph para pesquisar detalhes e fotos de contato. O valor padrão é `true`.  |
| seções | `object` -Configura quais seções são mostradas no cartão de pessoa.  |

### <a name="person-card-sections"></a>Seções de cartões de pessoa

O cartão de pessoa contém várias seções configuráveis para exibir os detalhes da pessoa:
* Contato – informações de contato, como email, telefone, cargo, local e muito mais.
* Organização-gráfico organizacional com gerentes, subordinados diretos e pessoas relevantes.
* Mensagens – mensagens de email mais relevantes com o usuário conectado no momento.
* Arquivos-arquivos compartilhados mais relevantes com o usuário conectado no momento.
* Profile-informações de perfil, como projetos, habilidades, idiomas e muito mais.

As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio da `MgtPersonCard.config.sections` propriedade Object. As propriedades a seguir estão disponíveis.

| Propriedade | Descrição |
| ------------ | ------------- |
| organization | `boolean` -Indica se a seção de organização de cartões de pessoa é exibida. O valor padrão é `true`.  |
| mailMessage | `boolean` -Indica se a seção mensagens de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| arquivos | `boolean` -Indica se a seção arquivos de cartão de pessoa é mostrada. O valor padrão é `true`.  |
| perfil | `boolean` -Indica se a seção de perfil de cartão de pessoa é mostrada. O valor padrão é `true`.  |

Para desabilitar uma seção, basta definir a propriedade como `false` em seu código de inicialização do aplicativo:.
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Configuração para integrações do teams

O componente Person-Card permite que o usuário entre em contato com a pessoa de destino, incluindo via chat do Microsoft Teams. Se estiver usando o componente dentro de um aplicativo de guia do Teams, você pode garantir que o componente se vincule diretamente a um chat, em vez de abrir uma janela do navegador, definindo o `microsoftTeamsLib` no `TeamsProvider` .

Se o componente de Person-Card não conseguir detectar a biblioteca do Teams, o componente tentará abrir o cliente da Web do teams.

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

Para obter mais informações sobre o `TeamsProvider` provedor, consulte [Microsoft Teams Provider](../providers/teams.md).

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-person` componente passará os detalhes da pessoa para o `mgt-person-card` componente. No entanto, você pode usar esses atributos para mudar isso ao padronizar o `mgt-person` componente ou ao usar o `mgt-person-card` componente como um componente autônomo.

| Atributo         | Tipo                     | Descrição                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| pessoa-detalhes | MicrosoftGraph. User <br> MicrosoftGraph. Person <br> MicrosoftGraph. Contact | Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário. |
| pessoa-imagem   | string                    | URI de imagem relacionado à pessoa exibida no cartão.                                   |
| Inherit-detalhes   | Nenhum.                  | Permite que o cartão de pessoa percorra a árvore pai para `mgt-person` que o componente use o mesmo `person-details` e os `person-image` dados.                      |
| ID de usuário | string | Permite que os desenvolvedores forneçam o ID de usuário para dados de recuperar exibidos no componente de cartão de pessoa |
| pessoa – consulta | string | Permite que os desenvolvedores forneçam uma consulta de pessoa para dados de recuperar exibidos no componente de cartão de pessoa |


## <a name="templates"></a>Modelos

O componente Person-Card usa [modelos](../customize-components/templates.md) que permitem que você adicione ou substitua partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| - | - | - |
| sem dados | null | O modelo usado quando não há dados disponíveis.
| Padrão. | `person`: O objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente pelo seu. |
| pessoa-detalhes | `person`: O objeto de detalhes da pessoa | O modelo usado para renderizar a parte superior do cartão Person. |
| adicional-detalhes | `person`: O objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo usado para adicionar conteúdo personalizado ao contêiner detalhes adicionais. |

Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão. 

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

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

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

Para saber mais, confira [estilos de componentes](../customize-components/style.md).

## <a name="microsoft-graph-apis-and-permissions"></a>APIs e permissões do Microsoft Graph

O controle Person-Card usa as seguintes APIs e permissões do Microsoft Graph.

| Recurso | Permissão | Seção |
| - | - | - |
| [/me](/graph/api/user-get) | User.Read | Padrão |
| [$value/me/Photo/](/graph/api/profilephoto-get) | User.Read | Padrão |
| [/me/People/? $search =](/graph/api/user-list-people) | People.Read | Padrão |
| [/me/contacts/\*](/graph/api/user-list-contacts) | Contacts.Read | Padrão |
| [/users/{id}](/graph/api/user-list-people) | User.ReadBasic.All | Padrão |
| [$value/Users/{ID}/Photo/](/graph/api/profilephoto-get) | User.ReadBasic.All | Padrão |
| [/me/presence](/graph/api/presence-get) | Presence.Read | Padrão |
| [/users/{id}/presence](/graph/api/presence-get) | Presence.Read.All | Padrão |
| [/users/{id}/manager](/graph/api/user-list-manager) | User.Read.All | Organização |
| [/users/{id}/directReports](/graph/api/user-list-directreports) | User.Read.All | Organização |
| [/users/{id}/people](/graph/api/user-list-people) | People.Read.All | Organização |
| [/me/messages](/graph/api/user-list-messages) | Mail.ReadBasic | Mensagens |
| [/me/insights/Shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used) | Sites.Read.All | Arquivos |
| [/users/{id}/profile](/graph/api/profile-get) | User.Read.All | Perfil |

A `MgtPersonCard` classe também expõe um `getScopes` método estático que retorna uma matriz de escopos necessários para que o cartão Person funcione com base na configuração do cartão de pessoa global.

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>Autenticação

O controle Person-Card usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md). 
