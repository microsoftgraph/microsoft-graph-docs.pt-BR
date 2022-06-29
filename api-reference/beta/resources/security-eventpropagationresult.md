---
title: Tipo de recurso eventPropagationResult
description: Representa o status de êxito de um evento criado e informações adicionais sobre os locais com escopo.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f8822b44020b2e76a41372b93f8bb71ee5f8bafe
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447536"
---
# <a name="eventpropagationresult-resource-type"></a>Tipo de recurso eventPropagationResult

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de uma solicitação de criação de evento de retenção e informações adicionais sobre os locais com escopo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|status|microsoft.graph.security.eventPropagationStatus|Indica o status da solicitação de criação de evento. Os valores possíveis são: `none`, `inProcessing`, `failed`, `success`.|
|statusInformation|Cadeia de caracteres|Informações adicionais sobre o status da solicitação de criação de evento.|
|serviceName|Cadeia de caracteres|O nome da carga de trabalho associada ao evento.|
|localização|Cadeia de caracteres|O nome do local específico na carga de trabalho associada ao evento.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventPropagationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventPropagationResult",
  "workload": "String",
  "location": "String",
  "status": "String",
  "statusInformation": "String"
}
```


