---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração para notificar automaticamente o remetente de um email de entrada com uma mensagem da '
localization_priority: Normal
ms.openlocfilehash: 81fb16a9124c60f43887150917f132579aa4f163
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569421"
---
# <a name="automaticrepliessetting-resource-type"></a>Tipo de recurso automaticRepliesSetting

Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails. 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|externalAudience|externalAudienceScope| O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`. Os valores possíveis são: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|string|A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.|
|internalReplyMessage|string|A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`. |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`. |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.|
|status|automaticRepliesStatus|Status de configurações de respostas automáticas. Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
