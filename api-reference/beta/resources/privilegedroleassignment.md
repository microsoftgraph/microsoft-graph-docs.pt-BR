---
title: tipo de recurso privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiada para um usuário específico. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: aef2b3962601a20df30f27c19ccd1abf23b0c561
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217901"
---
# <a name="privilegedroleassignment-resource-type"></a>tipo de recurso privilegedRoleAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma atribuição de função privilegiada para um usuário específico. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar privilegedRoleAssignment coleção](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection|Obtenha a coleção de objetos privilegedRoleAssignment.|
|[Get privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleAssignment.|
|[Criar tarefa](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Crie uma nova atribuição postando na coleção assignments.|
|[Delete](../api/privilegedroleassignment-delete.md) | None |Exclua um objeto privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Torne a atribuição de função como permanente.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Tornar a atribuição de função como qualificada.|
|[my](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md) collection|Obtenha as atribuições de função privilegiada do usuário atual.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|A data e hora UTC em que a atribuição de função privilegiada temporária será expirada. Para atribuição de função permanente, o valor é NULL.|
|id|string| O identificador exclusivo da atribuição de função privilegiada. Somente leitura. Ele está no formato de ' userId_roleId ', onde userId é a cadeia de caracteres GUID da ID de usuário do Azure AD e RoleID é a cadeia de caracteres GUID da ID da função de administrador do Azure.|
|iselevados|booliano|**true** se a atribuição de função é ativada. **false** se a atribuição de função é desativada.|
|resultMessage|string|Mensagem de resultado definida pelo serviço.|
|roleId|string|Identificador de função. Em formato de cadeia de caracteres GUID.|
|userId|cadeia de caracteres|Identificador de usuário. Em formato de cadeia de caracteres GUID.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Somente leitura. Anulável. As informações da função associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
