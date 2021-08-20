---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. accessReviewInstanceDecisionItemResource representa o recurso associado ao item de decisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4560882d117bde86da96a0d0d887fc7e2960b13d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264364"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso identificado por um objeto accessReviewInstanceDecisionItemResource. accessReviewInstanceDecisionItemResource é um tipo aberto que permite que outras propriedades sejam passadas.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do recurso|
|id|Cadeia de caracteres|ID do Recurso|
|type|Cadeia de caracteres|Tipo de recurso. Os tipos `Group` incluem: `ServicePrincipal` , , , , `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
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
