---
title: Tipo de recurso serviceHealth
description: Representa as informações de saúde de um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: f44a226375afa5af22b3413d84c47dd34dd473c8
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072499"
---
# <a name="servicehealth-resource-type"></a>Tipo de recurso serviceHealth

Namespace: microsoft.graph

Representa as informações de saúde de um serviço inscrito por um locatário.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceHealth](../api/servicehealth-get.md)|[serviceHealth](../resources/servicehealth.md)|Recupere as propriedades e as relações de um [objeto serviceHealth.](../resources/servicehealth.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do serviço.|
|service|Cadeia de caracteres|O nome do serviço. Use a [operação healthOverviews](../api/serviceannouncement-list-healthoverviews.md) de lista para obter nomes de cadeia de caracteres exatos para serviços inscritos pelo locatário.|
|status|serviceHealthStatus|Mostrar o status de saúde do serviço overral. Os valores possíveis são: `serviceOperational` , , , , , , , , `investigating` , , , `restoringService` , , `verifyingService` , , , `serviceRestored` , , `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` . `reported` `unknownFutureValue` Para obter mais detalhes, [consulte serviceHealthStatus values](../resources/servicehealthissue.md#servicehealthstatus-values).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|issues|Collection([serviceHealthIssue](../resources/servicehealthissue.md))|Uma coleção de problemas que aconteceram no serviço, com informações detalhadas para cada problema.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealth",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String",
  "id": "String (identifier)"
}
```

