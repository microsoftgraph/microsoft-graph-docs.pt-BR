---
title: Tipo de recurso privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiada para um usuário específico. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 62ecfd138aa4a0d3d7649f57ef7750a06381a557
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397471"
---
# <a name="privilegedroleassignment-resource-type-deprecated"></a>Tipo de recurso privilegedRoleAssignment (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Representa uma atribuição de função privilegiada para um usuário específico. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar coleção privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection|Obtenha a coleção de objetos privilegedRoleAssignment.|
|[Get privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Ler propriedades e relações do objeto privilegedRoleAssignment.|
|[Criar tarefa](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Crie uma nova atribuição postando na coleção de atribuições.|
|[Excluir](../api/privilegedroleassignment-delete.md) | Nenhum |Exclua um objeto privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Torne a atribuição de função como permanente.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Tornar a atribuição de função como qualificada.|
|[my](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md) collection|Obtenha as atribuições de função com privilégios do usuário atual.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|O DateTime UTC quando a atribuição de função com privilégios temporários expirará. Para atribuição de função permanente, o valor é nulo.|
|id|string| O identificador exclusivo para a atribuição de função com privilégios. Somente leitura. Ele está no formato de 'userId_roleId', em que userId é a cadeia de caracteres GUID para Azure AD id de usuário e roleId é a cadeia de caracteres GUID para a ID da função de administrador do Azure.|
|isElevated|booliano|**true** se a atribuição de função estiver ativada. **false** se a atribuição de função for desativada.|
|Resultmessage|string|Mensagem de resultado definida pelo serviço.|
|roleId|string|Identificador de função. No formato de cadeia de caracteres GUID.|
|userId|cadeia de caracteres|Identificador de usuário. No formato de cadeia de caracteres GUID.|

## <a name="relationships"></a>Relações
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


