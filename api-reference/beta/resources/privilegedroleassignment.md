---
title: Tipo de recurso privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiada para um usuário específico. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 5589f15c06cd91dca7f23a88cb3140bdc8c0e36c
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454077"
---
# <a name="privilegedroleassignment-resource-type"></a>Tipo de recurso privilegedRoleAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma atribuição de função privilegiada para um usuário específico. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar coleção privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection|Obter a coleção de objetos privilegedRoleAssignment.|
|[Get privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Ler propriedades e relações do objeto privilegedRoleAssignment.|
|[Criar tarefa](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Crie uma nova atribuição postando na coleção de atribuições.|
|[Delete](../api/privilegedroleassignment-delete.md) | Nenhum |Exclua um objeto privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Torne a atribuição de função como permanente.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Tornar a atribuição de função como qualificada.|
|[my](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md) collection|Obter as atribuições de função privilegiada do usuário atual.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|O UTC DateTime quando a atribuição de função privilegiada temporária será expirada. Para atribuição de função permanente, o valor é nulo.|
|id|string| O identificador exclusivo da atribuição de função privilegiada. Somente leitura. Está no formato de "userId_roleId", onde userId é a cadeia de caracteres GUID para id de usuário do Azure AD e roleId é a cadeia de caracteres GUID para id de função de administrador do Azure.|
|isElevated|booliano|**true** se a atribuição de função estiver ativada. **false** se a atribuição de função for desativada.|
|resultMessage|string|Mensagem de resultado definida pelo serviço.|
|roleId|string|Identificador de função. No formato de cadeia de caracteres GUID.|
|userId|cadeia de caracteres|Identificador de usuário. No formato de cadeia de caracteres GUID.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Somente leitura. Anulável. As informações de função associadas.|

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


