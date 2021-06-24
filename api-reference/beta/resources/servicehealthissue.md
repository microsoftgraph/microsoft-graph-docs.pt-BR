---
title: Tipo de recurso serviceHealthIssue
description: Representa um problema de saúde do serviço em um serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2436e6d0d5e49155b936cbfb7f7fc98630b7ce57
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109065"
---
# <a name="servicehealthissue-resource-type"></a>Tipo de recurso serviceHealthIssue

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um problema de saúde do serviço em um serviço.

O problema de saúde do serviço pode ser um incidente de serviço ou uma consultoria de serviço. Por exemplo:

* Incidente de serviço: "Exchange de caixa de correio está inobada".
* Aviso de serviço: "Os usuários podem ter atrasos na recepção de emails".

Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter serviceHealthIssue](../api/servicehealthissue-get.md)|[serviceHealthIssue](../resources/servicehealthissue.md)|Recupere as propriedades e as relações de um [objeto serviceHealthIssue.](../resources/servicehealthissue.md) |
|[Obter relatório de revisão pós-incidente](../api/servicehealthissue-incidentreport.md)|Stream|Fornece o documento de relatório de incidente pós-incidente (PIR) de um problema de serviço especificado para locatário. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classificação|serviceHealthClassificationType|O tipo de problema de saúde do serviço. Os valores possíveis são: `advisory`, `incident`, `unknownFutureValue`.|
|detalhes|Coleção([keyValuePair](../resources/keyvaluepair.md))|Detalhes adicionais sobre o problema de saúde do serviço. Essa propriedade não dá suporte a filtros. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|A hora de término do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|feature|String|O nome do recurso do problema do serviço.|
|featureGroup|String|O nome do grupo de recursos do problema do serviço.|
|id|String|A id do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|impactDescription|String|A descrição do impacto do problema do serviço.|
|isResolved|Booleano|Indica se o problema foi resolvido.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada do problema. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|origin|serviceHealthOrigin|Indica a origem do problema do serviço. Os valores possíveis são: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.|
|postagens|Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))|Coleção de postagens históricas para o problema do serviço.|
|service|Cadeia de caracteres|Indica o serviço afetado pelo problema.|
|startDateTime|DateTimeOffset|A hora de início do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|status|serviceHealthStatus|O status do problema do serviço. Os valores possíveis são: `serviceOperational` , , , , , , , , `investigating` , , , `restoringService` , , `verifyingService` , , , `serviceRestored` , , `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` . `reported` `unknownFutureValue`|
|title|String|O título do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssue",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "impactDescription": "String",
  "classification": "String",
  "origin": "String",
  "posts": [
    {
      "@odata.type": "microsoft.graph.serviceHealthIssuePost"
    }
  ],
  "status": "String",
  "service": "String",
  "feature": "String",
  "featureGroup": "String",
  "isResolved": "Boolean"
}
```

