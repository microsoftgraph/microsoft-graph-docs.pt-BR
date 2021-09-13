---
title: Tipo de recurso provisioningObjectSummary
description: Representa uma ação executada pelo serviço de Provisionamento do Azure AD e suas propriedades associadas.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ed38d1d2b3e29826c70d1e97b61227c5330e961d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143794"
---
# <a name="provisioningobjectsummary-resource-type"></a>Tipo de recurso provisioningObjectSummary

Namespace: microsoft.graph


Representa uma ação executada pelo serviço de Provisionamento do Azure AD e suas propriedades associadas. 

## <a name="methods"></a>Métodos

| Método  | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectsummary](provisioningobjectsummary.md) | Obter uma lista de todos os eventos de provisionamento que ocorreram em seu locatário. |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|provisioningAction|provisioningAction|Indica o nome da atividade ou o nome da operação. Os valores possíveis são: `create` , , , , e `update` `delete` `stageddelete` `disable` `other` `unknownFutureValue` . Para uma lista de atividades registradas, consulte a lista de atividades do Azure AD.|
|activityDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|changeId|String|ID exclusiva dessa alteração neste ciclo.|
|cycleId|String|ID exclusiva por iteração de trabalho.|
|durationInMilliseconds|Int32|Indica quanto tempo essa ação de provisionamento levou para ser final. Medido em milissegundos.|
|id|Cadeia de caracteres| Indica que a ID exclusiva para a atividade. Este é um GUID somente leitura.|
|initiatedBy|[Iniciador](initiator.md)|Detalhes de quem iniciou esse provisionamento.|
|jobId|String|A ID exclusiva para todo o trabalho de provisionamento.|
|ModifiedProperties|[Coleção modifiedProperty](modifiedproperty.md)|Detalhes de cada propriedade que foi modificada nesta ação de provisionamento neste objeto.|
|provisioningSteps|[Coleção provisioningStep](provisioningstep.md)|Detalhes de cada etapa no provisionamento.|
|servicePrincipal|[servicePrincipal](provisioningserviceprincipal.md) collection|Representa a entidade de serviço usada para provisionamento.|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|Detalhes do objeto de origem que está sendo provisionado.|
|sourceSystem|[provisioningSystem](provisioningsystem.md)|Detalhes do sistema de origem do objeto que está sendo provisionado.|
|provisioningStatusInfo|[provisioningStatusInfo](provisioningstatusinfo.md)|Detalhes do status do provisionamento.|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|Detalhes do objeto de destino que está sendo provisionado.|
|targetSystem|[provisioningSystem](provisioningsystem.md)|Detalhes do sistema de destino do objeto que está sendo provisionado.|
|tenantId|String|ID exclusiva do locatário do Azure AD.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


