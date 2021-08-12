---
title: Tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente chamando outro aplicativo ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 9da5a13e8e79de7a2f4bfb3405e96d3e577a9796cc0f2845e9d8c23fd9a3f53a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205945"
---
# <a name="approle-resource-type"></a>Tipo de recurso appRole

Namespace: microsoft.graph

Representa uma função de aplicativo que pode ser solicitada por (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada. 

Para adicionar, atualizar ou remover funções de aplicativo para um aplicativo, [atualize o aplicativo](../api/application-update.md) para o aplicativo ou serviço. As funções do aplicativo na entidade de aplicativo estarão disponíveis em todos os locatários onde o aplicativo é usado. Para definir funções de aplicativo que só são aplicáveis em seu locatário (por exemplo, funções [](../api/serviceprincipal-update.md) de aplicativo que representam funções personalizadas em sua instância de um aplicativo de vários locatários), você também pode atualizar a entidade de serviço do aplicativo, para adicionar ou atualizar funções de aplicativo à coleção **appRoles.**

Com [appRoleAssignments,](approleassignment.md)as funções do aplicativo podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|Especifica se essa função de aplicativo pode ser atribuída a usuários e grupos (definindo como ), para outro aplicativo (definindo como , ou `["User"]` `["Application"]` ambos (definindo como `["User", "Application"]` ). Funções de aplicativo que suportam a atribuição a entidades de serviço de outros aplicativos também são conhecidas como [permissões de aplicativo.](/graph/auth/auth-concepts#microsoft-graph-permissions) O valor "Application" só é suportado para funções de aplicativo definidas em **entidades de** aplicativo.|
|description|Cadeia de caracteres|A descrição da função de aplicativo. Isso é exibido quando a função do aplicativo está sendo atribuída e, se a função do aplicativo funcionar como uma permissão de aplicativo, durante experiências de consentimento.|
|displayName|Cadeia de caracteres|Nome de exibição para a permissão que aparece na atribuição de função de aplicativo e experiências de consentimento.|
|id|Guid|Identificador de função exclusivo dentro da **coleção appRoles.** Ao criar uma nova função de aplicativo, um novo identificador guid deve ser fornecido. |
|isEnabled|Booliano|Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão). Para excluir uma função, isso deve ser definido primeiro como **false**.  Nesse ponto, em uma chamada subsequente, essa função pode ser removida.|
|origin|Cadeia de caracteres| Especifica se a função de aplicativo é definida no objeto [application](application.md) ou na [entidade servicePrincipal.](serviceprincipal.md) Não _deve_ ser incluído em nenhuma solicitação POST ou PATCH. Somente leitura. |
|value|Cadeia de caracteres|Especifica o valor a ser incluído na declaração em tokens de ID e tokens de acesso autenticando um usuário ou entidade `roles` de serviço atribuído. Não deve exceder 120 caracteres de comprimento. Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` `A-Z` e `a-z` . Qualquer outro caractere, incluindo o caractere de espaço, não é permitido. Pode não começar com `.` . |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

