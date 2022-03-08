---
title: Tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente chamando outro aplicativo ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 8c9dfccaa9d41b78271f48119f3e23763232d0a6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337163"
---
# <a name="approle-resource-type"></a>Tipo de recurso appRole

Namespace: microsoft.graph

Representa uma função de aplicativo que pode ser solicitada por (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada. 

Para adicionar, atualizar ou remover funções de aplicativo para um aplicativo, [atualize o aplicativo](../api/application-update.md) para o aplicativo ou serviço. As funções do aplicativo na entidade de aplicativo estarão disponíveis em todos os locatários onde o aplicativo é usado. Para definir funções de aplicativo que só são aplicáveis em seu locatário (por exemplo, funções de aplicativo que representam funções personalizadas em sua instância de um aplicativo de vários [](../api/serviceprincipal-update.md) locatários), você também pode atualizar a entidade de serviço do aplicativo, para adicionar ou atualizar funções de aplicativo à coleção **appRoles**.

Com [appRoleAssignments](approleassignment.md), as funções do aplicativo podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowedMemberTypes|Coleção de cadeias de caracteres|Especifica se essa função de aplicativo pode ser atribuída a usuários e grupos ( `["User"]`definindo como ), para outro aplicativo ( `["Application"]`definindo como , ou ambos (definindo como `["User", "Application"]`). Funções de aplicativo que suportam a atribuição a entidades de serviço de outros aplicativos também são [conhecidas como permissões de aplicativo](/graph/auth/auth-concepts#microsoft-graph-permissions). O valor "Application" só é suportado para funções de aplicativo definidas em **entidades de** aplicativo.|
|descrição|String|A descrição da função de aplicativo. Isso é exibido quando a função do aplicativo está sendo atribuída e, se a função do aplicativo funcionar como uma permissão de aplicativo, durante experiências de consentimento.|
|displayName|String|Nome de exibição para a permissão que aparece na atribuição de função de aplicativo e experiências de consentimento.|
|id|Guid|Identificador de função exclusivo dentro da **coleção appRoles** . Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido. |
|isEnabled|Booliano|Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão). Para excluir uma função, isso deve ser definido primeiro como **false**.  Nesse ponto, em uma chamada subsequente, essa função pode ser removida.|
|origin|String| Especifica se a função de aplicativo é definida no objeto [application](application.md) ou na [entidade servicePrincipal](serviceprincipal.md) . Não _deve_ ser incluído em nenhuma solicitação POST ou PATCH. Somente leitura. |
|value|Cadeia de caracteres|Especifica o valor a ser incluído na `roles` declaração em tokens de ID e tokens de acesso autenticando um usuário ou entidade de serviço atribuído. Não deve exceder 120 caracteres de comprimento. Os caracteres permitidos `:` <code>&#96;</code> `]` `@` `^` `'` `&` `(` `%` `$` `#` `!` <code>&gt;</code> `?` `[` `;` `~`<code>&lt;</code> `}` `+` `*` `,` `/` `.` `)` `:` <code>&#124;</code> `+` `-` `{` `=` `_` são , bem como caracteres nos intervalos `0-9`e . `A-Z` `a-z` Qualquer outro caractere, incluindo o caractere de espaço, não é permitido. Pode não começar com `.`. |

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
  "allowedMemberTypes": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "value": "String"
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

