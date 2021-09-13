---
title: Tipo de recurso serviceHealthIssue
description: Representa um problema de saúde do serviço em um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b794284a4dafe16061faa5e84af9e72755d1f6b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019108"
---
# <a name="servicehealthissue-resource-type"></a>Tipo de recurso serviceHealthIssue

Namespace: microsoft.graph

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
|feature|Cadeia de caracteres|O nome do recurso do problema do serviço.|
|featureGroup|Cadeia de caracteres|O nome do grupo de recursos do problema do serviço.|
|id|Cadeia de caracteres|A id do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|impactDescription|String|A descrição do impacto do problema do serviço.|
|isResolved|Booliano|Indica se o problema foi resolvido.|
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

