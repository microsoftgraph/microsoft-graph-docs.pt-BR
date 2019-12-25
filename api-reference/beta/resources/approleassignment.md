---
title: Tipo de recurso plannerAssignment
description: Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário. Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica. Você pode criar, ler, atualizar e excluir as atribuições de função.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 34b9875efe231d734cd7ff3a8143d882ec3a87fb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870383"
---
# <a name="approleassignment-resource-type"></a>Tipo de recurso plannerAssignment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário. Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica. Você pode criar, ler, atualizar e excluir as atribuições de função.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência:  Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|Guid|A ID de função que foi atribuída à entidade.  Essa função deve ser declarada pela **resourceId** do aplicativo do recurso de destino em sua propriedade **appRoles**. Quando o recurso não declarar nenhuma permissão, uma ID padrão (zero GUID) deve ser especificada. Chave. Não anulável. |
|principalDisplayName|String|O nome de exibição da entidade à qual foi concedido o acesso.|
|principalId|Guid|O identificador exclusivo (**id**) da entidade à qual o acesso está sendo concedido. Obrigatório ao criar.            |
|principalType|String|O tipo de entidade.  Pode ser “User”, “Group” ou “ServicePrincipal”.|
|resourceDisplayName|String|O nome de exibição do recurso para o qual a tarefa foi feita.|
|resourceId|Guid|Identificador exclusivo (**id**) para o recurso de destino (entidade de serviço) para o qual a tarefa foi feita.|

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter appRoleAssignment](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |Leia propriedades e relações do objeto appRoleAssignment.|
|[Update](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |Atualize o objeto approleassignment. |
|[Delete](../api/approleassignment-delete.md) | Nenhum |Exclua o objeto appRoleAssignment. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
