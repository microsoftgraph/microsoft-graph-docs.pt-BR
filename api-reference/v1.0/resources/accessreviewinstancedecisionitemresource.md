---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Representa o recurso associado ao item de decisão.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3c51c0a4edf32bd090f78a6a921d0a246c0d33ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025626"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemResource

Namespace: microsoft.graph

Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. O objeto accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição do recurso|
|id|Cadeia de caracteres|Identificador do recurso|
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
