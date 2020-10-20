---
title: tipo de recurso serviceUserAgent
description: O tipo serviceUserAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 574fb733ad6d55a8cbdf36b8cf2de96bcaa8b8a6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601375"
---
# <a name="serviceuseragent-resource-type"></a>tipo de recurso serviceUserAgent

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um agente do usuário de serviço de um ponto de extremidade em uma chamada. Herda de tipo [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software do aplicativo usado por esse ponto de extremidade.|
|headerValue|String|Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.|
|role|Microsoft. Graph. callRecords. onrole|Identifica a função do serviço usado por esse ponto de extremidade. Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `unknown` `customBot` `skypeForBusinessMicrosoftTeamsGateway` `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` , `audioTeleconferencerController` , `skypeForBusinessUnifiedCommunicationApplicationPlatform` ,, `responseGroupServiceAnnouncementService` `gateway` , `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` ,,,,,.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "role": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

