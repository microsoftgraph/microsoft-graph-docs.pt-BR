---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 502bb1d376ca7534bcf967acfa5030e44540f86c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788133"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição do recurso|
|id|String|ID do Recurso|
|tipo|String|Tipo de recurso. Os tipos `Group` incluem: `ServicePrincipal` , , , , `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
