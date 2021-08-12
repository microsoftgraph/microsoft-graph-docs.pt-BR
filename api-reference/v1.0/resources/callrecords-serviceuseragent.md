---
title: Tipo de recurso serviceUserAgent
description: O tipo serviceUserAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bb8880b130c763599d75c5542725f1bb0fe850bad532693a62ee73ff25ffbfb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243627"
---
# <a name="serviceuseragent-resource-type"></a>Tipo de recurso serviceUserAgent

Namespace: microsoft.graph.callRecords

Representa um agente de usuário de serviço de um ponto de extremidade em uma chamada. Herda do [tipo userAgent.](callrecords-useragent.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationVersion|String|Identifica a versão do software de aplicativo usado por esse ponto de extremidade.|
|headerValue|Cadeia de caracteres|Valor de header do agente do usuário relatado por esse ponto de extremidade.|
|role|microsoft.graph.callRecords.serviceRole|Identifica a função do serviço usado por esse ponto de extremidade. Os valores possíveis são: `unknown` , , , , , , , , `customBot` `skypeForBusinessMicrosoftTeamsGateway` , , , `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` , `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` `audioTeleconferencerController` `skypeForBusinessUnifiedCommunicationApplicationPlatform` `responseGroupServiceAnnouncementService` `gateway` , `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` , .|

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
