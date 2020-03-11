---
title: tipo de recurso emailFileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo de email.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 29cb2f2f573f735504d2b54d4449109f82541f95
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591457"
---
# <a name="emailfileassessmentrequest-resource-type"></a>tipo de recurso emailFileAssessmentRequest

Usado para criar e recuperar uma avaliação de ameaça de arquivo de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).

O arquivo de email pode ser um tipo de arquivo. eml.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Create threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [emailFileAssessmentRequest](emailFileAssessmentRequest.md) | Crie uma nova solicitação de avaliação de arquivo de email postando um objeto **emailFileAssessmentRequest** . |
| [Get threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [emailFileAssessmentRequest](emailfileassessmentrequest.md) | Leia as propriedades e os relacionamentos de um objeto **emailFileAssessmentRequest** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|contentData|String|Conteúdo do arquivo de email codificado em base64. eml. O conteúdo do arquivo não pode buscar de volta porque não está armazenado.|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|A razão para emails roteados para seu destino. Os valores possíveis são `none`: `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.|
|recipientEmail|String|O destinatário de email cujas políticas são usadas para avaliar o email.|
|category|[threatCategory](enums.md#threatcategory-values)|A categoria da ameaça. Os valores possíveis são: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|O tipo de conteúdo de avaliação de ameaça. Os valores possíveis são: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|O criador da solicitação de avaliação de ameaças.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|A avaliação esperada do emissor. Os valores possíveis são: `block` e `unblock`.|
|id|String|A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).|
|objectrequest|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|A origem da solicitação de avaliação de ameaça. Os valores possíveis são: `user` e `administrator`.|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|O status do processo de avaliação. Os valores possíveis são: `pending`, `completed`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|resultados|coleção [threatAssessmentResult](threatassessmentresult.md)|Uma coleção de resultados de avaliação de ameaças. Somente leitura. Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "destinationRoutingReason": "String",
  "recipientEmail": "String",
  "category": "String",
  "contentType": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "id": "String (identifier)",
  "requestSource": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailFileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
