---
title: tipo de recurso serviceUserAgent
description: O tipo serviceUserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9cf6b0483ebda33068824f0a3345c12894fd2d7e
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353116"
---
# <a name="serviceuseragent-resource-type"></a><span data-ttu-id="b8d45-103">tipo de recurso serviceUserAgent</span><span class="sxs-lookup"><span data-stu-id="b8d45-103">serviceUserAgent resource type</span></span>

<span data-ttu-id="b8d45-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="b8d45-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8d45-105">Representa um agente do usuário de serviço de um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="b8d45-105">Represents a service user agent of an endpoint in a call.</span></span> <span data-ttu-id="b8d45-106">Herda de tipo [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="b8d45-106">Inherits from [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="b8d45-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8d45-107">Properties</span></span>

| <span data-ttu-id="b8d45-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8d45-108">Property</span></span>     | <span data-ttu-id="b8d45-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8d45-109">Type</span></span>        | <span data-ttu-id="b8d45-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8d45-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8d45-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="b8d45-111">applicationVersion</span></span>|<span data-ttu-id="b8d45-112">String</span><span class="sxs-lookup"><span data-stu-id="b8d45-112">String</span></span>|<span data-ttu-id="b8d45-113">Identifica a versão do software do aplicativo usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="b8d45-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="b8d45-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="b8d45-114">headerValue</span></span>|<span data-ttu-id="b8d45-115">String</span><span class="sxs-lookup"><span data-stu-id="b8d45-115">String</span></span>|<span data-ttu-id="b8d45-116">Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="b8d45-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="b8d45-117">role</span><span class="sxs-lookup"><span data-stu-id="b8d45-117">role</span></span>|<span data-ttu-id="b8d45-118">Microsoft. Graph. callRecords. onrole</span><span class="sxs-lookup"><span data-stu-id="b8d45-118">microsoft.graph.callRecords.serviceRole</span></span>|<span data-ttu-id="b8d45-119">Identifica a função do serviço usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="b8d45-119">Identifies the role of the service used by this endpoint.</span></span> <span data-ttu-id="b8d45-120">Os valores possíveis são: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b8d45-120">Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8d45-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8d45-121">JSON representation</span></span>

<span data-ttu-id="b8d45-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8d45-122">The following is a JSON representation of the resource.</span></span>

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