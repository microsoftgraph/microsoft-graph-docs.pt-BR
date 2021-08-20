---
title: Tipo de recurso serviceHealth
description: Representa as informações de saúde de um serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 89bc9579b6ca5af6b7306746394b439c83d40208
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266720"
---
# <a name="servicehealth-resource-type"></a>Tipo de recurso serviceHealth

Namespace: microsoft.graph

Representa as informações de saúde de um serviço inscrito por um locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceHealth](../api/servicehealth-get.md)|[serviceHealth](../resources/servicehealth.md)|Recupere as propriedades e as relações de um [objeto serviceHealth.](../resources/servicehealth.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do serviço.|
|service|Cadeia de caracteres|O nome do serviço. Use a [operação healthOverviews](../api/serviceannouncement-list-healthoverviews.md) de lista para obter nomes de cadeia de caracteres exatos para serviços inscritos pelo locatário.|
|status|serviceHealthStatus|Mostrar o status de saúde do serviço overral. Os valores possíveis são: `serviceOperational` , , , , , , , , `investigating` , , , `restoringService` , , `verifyingService` , , , `serviceRestored` , , `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` . `reported` `unknownFutureValue`|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|issues|Collection([serviceHealthIssue](../resources/servicehealthissue.md))|Uma coleção de problemas aconteceu no serviço, com informações detalhadas para cada problema.|

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

