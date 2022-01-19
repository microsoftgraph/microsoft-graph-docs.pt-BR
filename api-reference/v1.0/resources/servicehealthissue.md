---
title: Tipo de recurso serviceHealthIssue
description: Representa um problema de saúde do serviço em um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 7a005605a2994b21e21aa638e554bd8d24327b6a
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072555"
---
# <a name="servicehealthissue-resource-type"></a>Tipo de recurso serviceHealthIssue

Namespace: microsoft.graph

Representa um problema de saúde do serviço em um serviço.

O problema de saúde do serviço pode ser um incidente de serviço ou uma consultoria de serviço. Por exemplo:

* Incidente de serviço: "Exchange de caixa de correio está inobada".
* Aviso de serviço: "Os usuários podem ter atrasos na recepção de emails".

Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Methods
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
|impactDescription|Cadeia de caracteres|A descrição do impacto do problema do serviço.|
|isResolved|Booliano|Indica se o problema foi resolvido.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada do problema. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|origin|serviceHealthOrigin|Indica a origem do problema do serviço. Os valores possíveis são: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.|
|postagens|Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))|Coleção de postagens históricas para o problema do serviço.|
|service|Cadeia de caracteres|Indica o serviço afetado pelo problema.|
|startDateTime|DateTimeOffset|A hora de início do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|status|serviceHealthStatus|O status do problema do serviço. Os valores possíveis são: `serviceOperational` , , , , , , , , `investigating` , , , `restoringService` , , `verifyingService` , , , `serviceRestored` , , `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` . `reported` `unknownFutureValue` Confira mais na [tabela abaixo](#servicehealthstatus-values).|
|title|Cadeia de caracteres|O título do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|

### <a name="servicehealthstatus-values"></a>valores serviceHealthStatus
|Member|Descrição|
|:---|:---|
|serviceOperational|O serviço é ável e nenhum problema foi identificado.|
|investigar|Um possível problema foi identificado e mais informações estão sendo coletadas sobre o que está acontecendo e o escopo do impacto.|
|restoringService|A causa do problema foi identificada e ações estão sendo tomadas para trazer o serviço de volta a um estado saudável.|
|verifyingService|A ação foi tomada para atenuar o problema e estamos verificando se o serviço está bem.|
|serviceRestored|A ação corretiva resolveu o problema subjacente e o serviço foi restaurado para um estado corretamente. Para descobrir o que deu errado, confira os detalhes do problema.|
|postIncidentReviewPublished|Um relatório pós-incidente para um problema específico que inclui informações de causa raiz foi publicado, com as próximas etapas para garantir que um problema semelhante não se recidiva.|
|serviceDegradation|Um problema é confirmado que pode afetar o uso de um serviço ou recurso. Talvez você veja esse status se um serviço apresentar um desempenho mais lento do que o normal, se houver interrupções intermitentes ou se um recurso não estiver funcionando, por exemplo.|
|serviceInterruption|Você verá esse status se um problema for determinado para afetar a capacidade dos usuários de acessar o serviço. Neste caso, a questão é significativa e pode ser reproduzida de forma consistente.|
|extendedRecovery|Esse status indica que a ação corretiva está em andamento para restaurar o serviço para a maioria dos usuários, mas levará algum tempo para alcançar todos os sistemas afetados. Você também poderá ver esse status se uma correção temporária for feita para reduzir o impacto enquanto uma correção permanente aguarda a aplicação.|
|falsePositive|Após uma investigação detalhada, o serviço é confirmado como saudável e operacional conforme projetado. Nenhum impacto no serviço foi observado ou a causa do incidente foi criada fora do serviço. Incidentes e avisos com esse status aparecem na exibição de histórico até expirarem (após o período de tempo indicado na postagem final desse evento).|
|investigationSuspended|Se nossa investigação detalhada de um possível problema resulta em uma solicitação de informações adicionais dos clientes para permitir que a equipe de serviço investigue mais, você verá esse status. Se a equipe de serviço precisar que você aja, elas permitirão que você saiba de que dados ou logs eles precisam.|
|resolvido|O status Windows de serviço da Microsoft que corresponde ao serviço restaurado.|
|mitigatedExternal|O Windows de serviço que corresponde à restauração do serviço.|
|mitigado|O Windows de serviço que corresponde à recuperação estendida.|
|resolvedExternal|O Windows de serviço que corresponde à investigação suspensa.|
|confirmed|O Windows de serviço que corresponde à interrupção do serviço.|
|reportado|O Windows de serviço que corresponde à investigação.|

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

