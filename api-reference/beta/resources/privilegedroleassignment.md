---
title: tipo de recurso de privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiado para um usuário específico. '
localization_priority: Normal
ms.openlocfilehash: ec6bc34ecd56839c764592ff298475e8648f300b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823314"
---
# <a name="privilegedroleassignment-resource-type"></a>tipo de recurso de privilegedRoleAssignment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma atribuição de função privilegiado para um usuário específico. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Coleção de privilegedRoleAssignment de lista](../api/privilegedroleassignment-list.md) | coleção [privilegedRoleAssignment](privilegedroleassignment.md)|Obtenha a coleção de objetos privilegedRoleAssignment.|
|[Obter privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleAssignment.|
|[Criar atribuição](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Crie uma nova atribuição de lançamento para a coleção assignments.|
|[Delete](../api/privilegedroleassignment-delete.md) | Nenhum |Exclua objeto privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Fazer a atribuição de função como permanente.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Fazer a atribuição de função como qualificado.|
|[Minha](../api/privilegedroleassignment-my.md)|coleção [privilegedRoleAssignment](privilegedroleassignment.md)|Obtenha as atribuições de função privilegiado do usuário atual.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|DateTime UTC quando a atribuição de função privilegiado temporário será expirada. Para atribuição de função permanente, o valor é nulo.|
|id|string| O identificador exclusivo para a atribuição de função privilegiado. Somente leitura. É no formato de 'userId_roleId', onde userId é a cadeia de caracteres do GUID para id de usuário do Windows Azure AD e roleId é a cadeia de caracteres do GUID para id de função de administrador do Azure.|
|isElevated|booliano|**true** se a atribuição de função é ativada. **false** se a atribuição de função é desativada.|
|resultMessage|string|Mensagem de resultado definido pelo serviço.|
|roleId|string|Identificador de função. No formato de cadeia de caracteres GUID.|
|userId|string|Identificador de usuário. No formato de cadeia de caracteres GUID.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Somente leitura. Anulável. As informações de função associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
