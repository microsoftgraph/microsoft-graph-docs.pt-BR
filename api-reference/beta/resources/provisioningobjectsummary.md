---
title: tipo de recurso provisioningObjectSummary
description: Representa uma ação executada pelo serviço de provisionamento do Azure AD e suas propriedades associadas.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eabbb0c0cd1cd692ad6ebc5a346c46473161b1
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394593"
---
# <a name="provisioningobjectsummary-resource-type"></a>tipo de recurso provisioningObjectSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação executada pelo serviço de provisionamento do Azure AD e suas propriedades associadas. 

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectSummary](provisioningobjectsummary.md) | Obtenha uma lista de todos os eventos de provisionamento que ocorreram em seu locatário. |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ação|String|Indica o nome da atividade ou o nome da operação (por exemplo, criar usuário, Adicionar membro ao grupo). Para obter uma lista de atividades registradas, consulte lista de atividades do Azure AD.|
|activityDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|ChangeId|String|ID exclusiva dessa alteração nesse ciclo.|
|cycleid|String|ID exclusiva por iteração de trabalho.|
|durationInMilliseconds|Int32|Indica quanto tempo esta ação de provisionamento levou para ser concluída. Medido em milissegundos.|
|id|Cadeia de caracteres| Indica que a ID exclusiva para a atividade. Este é um GUID somente leitura.|
|initiatedBy|[Iniciador](initiator.md)|Detalhes sobre quem iniciou este provisionamento.|
|ID|String|A identificação exclusiva de todo o trabalho de provisionamento.|
|ModifiedProperties|coleção [modifiedproperty](modifiedproperty.md)|Os detalhes de cada propriedade que foi modificada nesta ação de provisionamento neste objeto.|
|provisioningSteps|coleção [provisioningStep](provisioningstep.md)|Detalhes de cada etapa no provisionamento.|
|servicePrincipal|[servicePrincipal](serviceprincipal.md) collection|Representa a entidade de serviço usada para provisionamento.|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|Detalhes do objeto de origem que está sendo provisionado.|
|sourceSystem|[provisioningSystemDetails](provisioningsystemdetails.md)|Detalhes do sistema de origem do objeto que está sendo provisionado.|
|statusInfo|[statusBase](statusbase.md)|Detalhes do status de provisionamento.|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|Detalhes do objeto de destino que está sendo provisionado.|
|targetSystem|[provisioningSystemDetails](provisioningsystemdetails.md)|Detalhes do sistema de destino do objeto que está sendo provisionado.|
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
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
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
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
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
