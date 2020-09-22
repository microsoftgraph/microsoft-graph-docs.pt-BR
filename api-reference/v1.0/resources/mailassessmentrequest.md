---
title: tipo de recurso mailAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de email.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c684694ac2af189698c74935ca58f70aa4a8cf9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083075"
---
# <a name="mailassessmentrequest-resource-type"></a>tipo de recurso mailAssessmentRequest

Usado para criar e recuperar uma avaliação de ameaça de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).

Quando você cria uma solicitação de avaliação de ameaça de email, os emails devem ser recebidos pelo usuário especificado em `recipientEmail` . Permissões de [email](/graph/permissions-reference#mail-permissions) delegadas (mail. Read ou mail. Read. Shared) são requried para acessar as mensagens recebidas pelo usuário ou compartilhadas por outra pessoa.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Create threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [mailAssessmentRequest](mailAssessmentRequest.md) | Crie uma nova solicitação de avaliação de email postando um objeto **mailAssessmentRequest** . |
| [Get threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [mailAssessmentRequest](mailassessmentrequest.md) | Leia as propriedades e os relacionamentos de um objeto **mailAssessmentRequest** . |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|A razão para emails roteados para seu destino. Os valores possíveis são:, `none` `mailFlowRule` , `safeSender` , `blockedSender` , `advancedSpamFiltering` , `domainAllowList` , `domainBlockList` , `notInAddressBook` , `firstTimeSender` , `autoPurgeToInbox` , `autoPurgeToJunk` , `autoPurgeToDeleted` ,, `outbound` `notJunk` `junk` .|
|messageUri|Cadeia de caracteres|O URI do recurso da mensagem de email para avaliação.|
|recipientEmail|Cadeia de caracteres|O destinatário de email cujas políticas são usadas para avaliar o email.|
|category|[threatCategory](enums.md#threatcategory-values)|A categoria da ameaça. Os valores possíveis são: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|O tipo de conteúdo de avaliação de ameaça. Os valores possíveis são: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|O criador da solicitação de avaliação de ameaças.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|A avaliação esperada do emissor. Os valores possíveis são: `block` e `unblock`.|
|id|Cadeia de caracteres|A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).|
|objectrequest|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|A origem da solicitação de avaliação de ameaça. Os valores possíveis são: `user` e `administrator`.|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|O status do processo de avaliação. Os valores possíveis são: `pending`, `completed`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|resultados|coleção [threatAssessmentResult](threatassessmentresult.md)|Uma coleção de resultados de avaliação de ameaças. Somente leitura. Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você a aplique `$expand` .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "destinationRoutingReason": "String",
  "messageUri": "String",
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
  "description": "mailAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

