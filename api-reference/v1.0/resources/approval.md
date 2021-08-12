---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b2917825104d30813f6ad98237dd68492e4a269481d1013458edb1038208430c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212218"
---
# <a name="approval-resource-type"></a>tipo de recurso de aprovação

Namespace: microsoft.graph

Representa o objeto de aprovação para decisões associadas a uma solicitação.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da decisão de aprovação.|
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
