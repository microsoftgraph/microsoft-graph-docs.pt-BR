---
title: Tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente chamando outro aplicativo ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f61eca3971baeb426f4a20697a1e7ffca74e5071
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132472"
---
# <a name="approle-resource-type"></a>Tipo de recurso appRole

Namespace: microsoft.graph

Representa uma função de aplicativo que pode ser solicitada (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada. 

A **propriedade appRoles** do [aplicativo e](application.md) [entidades servicePrincipal](serviceprincipal.md) são uma coleção de **appRole**. 

Com [appRoleAssignments,](approleassignment.md)as funções de aplicativo podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|Especifica se essa função de aplicativo pode ser atribuída a usuários e grupos (configurando como ), para outro aplicativo (configurando para , ou `["User"]` `["Application"]` ambos (definindo como `["User", "Application"]` ). Funções de aplicativo que suportam a atribuição a entidades de serviço de outros aplicativos também são conhecidas como [permissões de aplicativo.](/graph/auth/auth-concepts#microsoft-graph-permissions) O valor "Aplicativo" só tem suporte para funções de aplicativo definidas em **entidades** de aplicativo.|
|description|String|A descrição da função do aplicativo. Isso é exibido quando a função de aplicativo está sendo atribuída e, se a função de aplicativo funciona como uma permissão de aplicativo, durante experiências de consentimento.|
|displayName|String|Nome de exibição da permissão que aparece na atribuição de função de aplicativo e experiências de consentimento.|
|id|Guid|Identificador de função exclusivo dentro da **coleção appRoles.** Ao criar uma nova função de aplicativo, um novo identificador Guid deve ser fornecido. |
|isEnabled|Booliano|Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **verdadeiro** (que é o padrão). Para excluir uma função, primeiro deve ser definido como **false**.  Nesse ponto, em uma chamada subsequente, essa função pode ser removida.|
|origin|String| Especifica se a função de aplicativo é definida no [objeto de](application.md) aplicativo ou na [entidade servicePrincipal.](serviceprincipal.md) Não _deve ser_ incluído em solicitações POST ou PATCH. Somente leitura. |
|value|Cadeia de caracteres|Especifica o valor a ser incluído na declaração em tokens de ID e tokens de acesso autenticando um usuário atribuído ou entidade `roles` de serviço. Não deve exceder 120 caracteres de comprimento. Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` e `A-Z` `a-z` . Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.  |

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

