---
title: Tipo de recurso mailboxSettings
description: Configurações para a caixa de correio principal do usuário conectado.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4a6e053e60616464c8d1f3facc5394398a2346e5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089330"
---
# <a name="mailboxsettings-resource-type"></a>Tipo de recurso mailboxSettings

Namespace: microsoft.graph

Configurações para a caixa de correio principal de um [usuário](user.md).

Você pode [obter](../api/user-get-mailboxsettings.md) ou [atualizar](../api/user-update-mailboxsettings.md) as configurações de caixa de correio de um usuário consultando a propriedade **mailboxSettings** do usuário.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|archiveFolder|string|ID de uma pasta de arquivo morto do usuário.|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.|
|dateFormat|cadeia de caracteres|O formato de data para a caixa de correio do usuário.|
|delegateMeetingMessageDeliveryOptions|delegateMeetingMessageDeliveryOptions| Se o usuário tiver um representante de calendário, isso especifica se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas de reunião. Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.|
|idioma|[localeInfo](localeinfo.md)|Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.|
|timeFormat|cadeia de caracteres|O formato de hora da caixa de correio do usuário.|
|timeZone|string|O fuso horário padrão para a caixa de correio do usuário.|
|workingHours|[workingHours](workinghours.md)|Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.|

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
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

