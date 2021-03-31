---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6d41146551586f681ebf5ed7fda735151f1efc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469511"
---
# <a name="approval-resource-type"></a>tipo de recurso de aprovação

Namespace: microsoft.graph

Representa o objeto de aprovação para decisões associadas a uma solicitação.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador da decisão de aprovação.|
|Estágios|[coleção approvalStage](../resources/approvalstage.md)|Uma coleção de estágios na decisão de aprovação. |

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|Estágios|[coleção approvalStage](../resources/approvalstage.md)|Uma coleção de estágios na decisão de aprovação. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```
