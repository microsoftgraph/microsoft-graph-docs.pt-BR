---
title: Tipo de recurso serviceHealthIssue
description: Representa um problema de saúde do serviço em um serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 9126ca6ed06ce096d2748b7c01a9a61359099656
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291271"
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
|[Obter serviceHealthIssue](../api/servicehealthissue-get.md)|[serviceHealthIssue](../resources/servicehealthissue.md)|Recupere as propriedades e as relações de um [objeto serviceHealthIssue](../resources/servicehealthissue.md) . |
|[Obter relatório de revisão pós-incidente](../api/servicehealthissue-incidentreport.md)|Stream|Obter o documento de relatório de incidente pós-incidente (PIR) de um problema de serviço especificado para locatário. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classificação|serviceHealthClassificationType|O tipo de problema de saúde do serviço. Os valores possíveis são: `advisory`, `incident`, `unknownFutureValue`.|
|detalhes|Collection([keyValuePair](../resources/keyvaluepair.md))|Detalhes adicionais sobre o problema de saúde do serviço. Essa propriedade não dá suporte a filtros. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|A hora de término do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|feature|Cadeia de caracteres|O nome do recurso do problema do serviço.|
|featureGroup|Cadeia de caracteres|O nome do grupo de recursos do problema do serviço.|
|id|String|A id do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|impactDescription|Cadeia de caracteres|A descrição do impacto do problema do serviço.|
|isResolved|Booliano|Indica se o problema foi resolvido.|
|lastModifiedDateTime|DateTimeOffset|A última hora modificada do problema. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|origin|serviceHealthOrigin|Indica a origem do problema do serviço. Os valores possíveis são: `microsoft`, `thirdParty`, `customer`, `unknownFutureValue`.|
|postagens|Collection([serviceHealthIssuePost](../resources/servicehealthissuepost.md))|Coleção de postagens históricas para o problema do serviço.|
|service|Cadeia de caracteres|Indica o serviço afetado pelo problema.|
|startDateTime|DateTimeOffset|A hora de início do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|status|serviceHealthStatus|O status do problema do serviço. Os valores possíveis são: , , , , `serviceRestored``verifyingService`, , `postIncidentReviewPublished`, , `serviceInterruption``serviceDegradation``extendedRecovery`, , `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, , `mitigated`, , `resolvedExternal`, , . `reported``unknownFutureValue``confirmed``restoringService``investigating``serviceOperational` Para obter mais detalhes, consulte [valores serviceHealthStatus](#servicehealthstatus-values).|
|title|Cadeia de caracteres|O título do problema do serviço. Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).|

### <a name="servicehealthstatus-values"></a>valores serviceHealthStatus
|Member|Descrição|
|:---|:---|
|serviceOperational|O serviço é ável e nenhum problema foi identificado.|
|investigar|Um possível problema foi identificado e mais informações estão sendo coletadas sobre o que está acontecendo e o escopo do impacto.|
|restoringService|A causa do problema foi identificada e ações estão sendo tomadas para trazer o serviço de volta a um estado  saudável.|
|verifyingService|A ação foi tomada para atenuar o problema e estamos verificando se o serviço está  bem.|
|serviceRestored|A ação corretiva resolveu o problema subjacente e o serviço foi restaurado para um estado corretamente. Para descobrir o que deu errado, confira os detalhes do problema.|
|postIncidentReviewPublished|Um relatório pós-incidente para um problema específico que inclui informações de causa raiz foi publicado, com as próximas etapas para garantir que um problema semelhante não se recidiva.|
|serviceDegradation|Um problema é confirmado que pode afetar o uso de um serviço ou recurso. Talvez você veja esse status se um serviço apresentar um desempenho mais lento do que o normal, se houver interrupções intermitentes ou se um recurso não estiver funcionando, por exemplo.|
|serviceInterruption|Você verá esse status se um problema for determinado para afetar a capacidade dos usuários de acessar o serviço. Neste caso, a questão é significativa e pode ser reproduzida de forma consistente.|
|extendedRecovery|Esse status indica que a ação corretiva está em andamento para restaurar o serviço para a maioria dos usuários, mas levará algum tempo para alcançar todos os sistemas afetados. Você também poderá ver esse status se uma correção temporária for feita para reduzir o impacto enquanto uma correção permanente aguarda a aplicação.|
|falsePositive|Após uma investigação detalhada, o serviço é confirmado como saudável e operacional conforme projetado. Nenhum impacto no serviço foi observado ou a causa do incidente foi criada fora do serviço. Incidentes e avisos com esse status aparecem na exibição de histórico até expirarem (após o período de tempo indicado na postagem final desse evento).|
|investigationSuspended|Se nossa investigação detalhada de um possível problema resulta em uma solicitação de informações adicionais dos clientes para permitir que a equipe de serviço investigue mais, você verá esse status. Se a equipe de serviço precisar que você aja, elas permitirão que você saiba de que dados ou logs eles precisam.|
|resolvido|Reserved for future use.|
|mitigatedExternal|Reserved for future use.|
|mitigado|Reserved for future use.|
|resolvedExternal|Reserved for future use.|
|confirmed|Reserved for future use.|
|reportado|Reserved for future use.|


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

