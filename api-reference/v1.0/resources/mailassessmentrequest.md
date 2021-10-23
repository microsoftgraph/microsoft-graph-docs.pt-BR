---
title: Tipo de recurso mailAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de email.
ms.localizationpriority: medium
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 83a2fb0fa5a309d880830a11f9806a729383b1d7
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560825"
---
# <a name="mailassessmentrequest-resource-type"></a>Tipo de recurso mailAssessmentRequest

Usado para criar e recuperar uma avaliação de ameaça de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).

Quando você cria uma solicitação de avaliação de ameaça de email, o email deve ser recebido pelo usuário especificado em `recipientEmail` . As permissões [de email delegadas](/graph/permissions-reference#mail-permissions) (Mail.Read ou Mail.Read.Shared) são requriadas para acessar o email recebido pelo usuário ou compartilhado por outra pessoa.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Create threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [mailAssessmentRequest](mailAssessmentRequest.md) | Crie uma nova solicitação de avaliação de email postando um **objeto mailAssessmentRequest.** |
| [Get threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [mailAssessmentRequest](mailassessmentrequest.md) | Leia as propriedades e as relações de um **objeto mailAssessmentRequest.** |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|O motivo do email roteado para seu destino. Os valores possíveis são: `none` , , , , , , , , , `mailFlowRule` , , `safeSender` , , , `blockedSender` `advancedSpamFiltering` `domainAllowList` , `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` .|
|messageUri|Cadeia de Caracteres|O URI de recurso da mensagem de email para avaliação.|
|recipientEmail|Cadeia de Caracteres|O destinatário de email cujas políticas são usadas para avaliar o email.|
|category|[threatCategory](enums.md#threatcategory-values)|A categoria de ameaça. Os valores possíveis são: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|O tipo de conteúdo da avaliação de ameaças. Os valores possíveis são: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|O criador da solicitação de avaliação de ameaças.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|A avaliação esperada do enviador. Os valores possíveis são: `block` e `unblock`.|
|id|Cadeia de caracteres|A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|A origem da solicitação de avaliação de ameaças. Os valores possíveis são: `administrator` .|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|O status do processo de avaliação. Os valores possíveis são: `pending`, `completed`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|results|[Coleção threatAssessmentResult](threatassessmentresult.md)|Uma coleção de resultados de avaliação de ameaças. Somente leitura. Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
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

