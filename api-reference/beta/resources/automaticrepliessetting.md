---
title: Tipo de recurso automaticRepliesSetting
description: 'Definições de configuração automaticamente notificar o remetente de um email de entrada com uma mensagem a partir do '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820654"
---
# <a name="automaticrepliessetting-resource-type"></a>Tipo de recurso automaticRepliesSetting

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Por exemplo, uma resposta automática para notificar que o usuário conectado está disponível para responder a emails. 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|externalAudience|String| O conjunto da audiência externa para a organização do usuário conectado que receberá **ExternalReplyMessage**, se **Status** for `AlwaysEnabled` ou `Scheduled`. Os valores possíveis são: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|string|A resposta automática para enviar à audiência externa especificada, se **Status** for `AlwaysEnabled` ou `Scheduled`.|
|internalReplyMessage|string|A resposta automática para enviar à audiência interna na organização do usuário conectado, se **Status** for `AlwaysEnabled` ou `Scheduled`. |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data e a hora em que as respostas automáticas estão definidas para terminar, se **Status** está definido como `Scheduled`. |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data e a hora em que as respostas automáticas estão definidas para começar, se **Status** está definido como `Scheduled`.|
|status|Cadeia de caracteres|Status de configurações de respostas automáticas. Os valores possíveis são: `disabled`, `alwaysEnabled`, `scheduled`.|

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
