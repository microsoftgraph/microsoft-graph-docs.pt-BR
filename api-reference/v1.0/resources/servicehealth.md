---
title: Tipo de recurso serviceHealth
description: Representa as informações de saúde de um serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 254702516d536617ef5afa114bc7a41761ce3499a932b4c7e2d8560ac7f92441
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195583"
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
|id|String|A ID do serviço.|
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

