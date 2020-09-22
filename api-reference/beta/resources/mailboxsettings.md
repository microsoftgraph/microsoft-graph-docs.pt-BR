---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c3ff60d591257929d2856720ad298231d2afb944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095016"
---
# <a name="mailboxsettings-resource-type"></a>Tipo de recurso mailboxSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações da caixa de correio principal de um [usuário](user.md).

Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|archiveFolder|string|ID de uma pasta de arquivo morto do usuário. Somente leitura.|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.|
|dateFormat|cadeia de caracteres|O formato de data da caixa de correio do usuário.|
|delegateMeetingMessageDeliveryOptions|delegateMeetingMessageDeliveryOptions| Se o usuário tiver um representante de calendário, isso especificará se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas da reunião. Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`. O padrão é `sendToDelegateOnly` .|
|idioma|[localeInfo](localeinfo.md)|Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.|
|Formato de TimeFormat|cadeia de caracteres|O formato de hora da caixa de correio do usuário.|
|timeZone|string|O fuso horário padrão para a caixa de correio do usuário.|
|workingHours|[workingHours](workinghours.md)|Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.|
|userpurpose|[userpurpose](userpurpose.md)|O objetivo da caixa de correio. Usado para diferenciar uma caixa de correio de um único usuário de uma caixa de correio compartilhada e caixa de correio de equipamento no Exchange Online. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "dateFormat": "string",
  "delegateMeetingMessageDeliveryOptions": "String",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"},
  "userPurpose": {"@odata.type": "microsoft.graph.userPurpose"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


