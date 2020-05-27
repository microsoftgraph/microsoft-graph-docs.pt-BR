---
title: tipo de recurso appRole
description: Representa uma função de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 8505380b50e32e9c996f960ab2343efa7e372e4a
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383767"
---
# <a name="approle-resource-type"></a>tipo de recurso appRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de aplicativo que pode ser solicitada por (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada. 

A propriedade **appRoles** das entidades [Application](application.md) e [servicePrincipalName](serviceprincipal.md) é uma coleção de **appRole**. 

Com o [appRoleAssignments](approleassignment.md), as funções de aplicativo podem ser atribuídas a usuários, grupos ou a entidades de serviço de outros aplicativos.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowedMemberTypes|Conjunto de cadeias de caracteres|Especifica se esta função de aplicativo pode ser atribuída a usuários e grupos (definindo como `["User"]` ), a outros aplicativos (por configuração `["Application"]` ou ambos (por meio da configuração `["User", "Application"]` ). Funções de aplicativo que dão suporte à atribuição de entidades de serviço de outros aplicativos também são conhecidas como [permissões de aplicativo](/graph/auth/auth-concepts#microsoft-graph-permissions).|
|description|String|A descrição da função de aplicativo. Isso é exibido quando a função de aplicativo está sendo atribuída e, se a função de aplicativo funciona como uma permissão de aplicativo, durante experiências de consentimento.|
|displayName|Cadeia de caracteres|Nome para exibição da permissão que aparece nas experiências de consentimento e atribuição de função de aplicativo.|
|id|Guid|Identificador de função exclusivo dentro da coleção **appRoles** . Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido. |
|isEnabled|Boolean|Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão). Para excluir uma função, é necessário primeiro defini-la como **false**.  Nesse ponto, em uma chamada subsequente, essa função pode ser removida.|
|tenham|String| Especifica se a função de aplicativo é definida no objeto [Application](application.md) ou na entidade [servicePrincipalName](serviceprincipal.md) . _Não_ deve ser incluído em solicitações POST ou patch. Somente leitura. |
|value|Cadeia de caracteres|Especifica o valor a ser incluído na `roles` declaração em tokens de ID e tokens de acesso Autenticando um usuário atribuído ou uma entidade de serviço. Não deve exceder 120 caracteres de comprimento. Os caracteres permitidos são `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , bem como os caracteres nos intervalos `0-9` `A-Z` e `a-z` . Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.  |

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
