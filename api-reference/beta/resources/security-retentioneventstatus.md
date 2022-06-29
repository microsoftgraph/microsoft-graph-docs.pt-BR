---
title: Tipo de recurso retentionEventStatus
description: Para retenção baseada em evento, fornece o status da propagação do evento para os locais especificados após a criação do evento.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d21fabd92f19ac1be107568426e0c3e116e6a7ea
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447520"
---
# <a name="retentioneventstatus-resource-type"></a>Tipo de recurso retentionEventStatus

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para retenção baseada em evento, esse atributo fornece o status da propogação de evento para os locais de destino após a criação do evento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|[microsoft.graph.publicError](../resources/publicerror.md)|O erro se o status não for bem-sucedido.|
|status|microsoft.graph.security.eventStatusType|O status da distribuição. Os valores possíveis são: `pending`, `error`, `success`, `notAvaliable`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionEventStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEventStatus",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "status": "String"
}
```

