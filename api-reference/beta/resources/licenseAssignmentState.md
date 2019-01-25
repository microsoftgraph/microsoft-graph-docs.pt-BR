---
title: tipo de recurso de licenseAssignmentState
description: 'A propriedade **licenseAssignmentStates** da entidade do usuário é uma coleção de **licenseAssignmentState**. Ela fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes inclui informações como:  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515276"
---
# <a name="licenseassignmentstate-resource-type"></a>tipo de recurso de licenseAssignmentState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **licenseAssignmentStates** da entidade do [usuário](user.md) é uma coleção de **licenseAssignmentState**. Ela fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes inclui informações como:  

 - Quais planos estão desabilitados para um usuário
 - Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
 - Estado atual da atribuição
 - Se o estado de atribuição for erro, o que é detalhes do erro da falha? 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|string|A identificação do grupo que atribui essa licença. Se a atribuição for uma licença atribuído diretamente, esse campo será Null. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que serão desabilitados nessa atribuição. Somente Leitura.|
|erro|String|Erro de falha de atribuição de licença. Se a licença foi distribuída com êxito, esse campo será Null. Somente Leitura. Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, e `Others`. Para obter mais informações sobre como identificar e resolver a atribuição de licença erros consulte [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|estado|String|Indica o estado atual dessa atribuição. Somente Leitura. Valores possíveis: ativo, ActiveWithError, desabilitado e erro.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
