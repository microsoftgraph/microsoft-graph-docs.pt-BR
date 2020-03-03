---
title: tipo de recurso serviceUserAgent
description: O tipo serviceUserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c8cfe517b127bcdf359c69ab600146593f5ef288
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394656"
---
# <a name="serviceuseragent-resource-type"></a><span data-ttu-id="a88f3-103">tipo de recurso serviceUserAgent</span><span class="sxs-lookup"><span data-stu-id="a88f3-103">serviceUserAgent resource type</span></span>

<span data-ttu-id="a88f3-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="a88f3-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a88f3-105">Representa um agente do usuário de serviço de um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a88f3-105">Represents a service user agent of an endpoint in a call.</span></span> <span data-ttu-id="a88f3-106">Herda de tipo [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="a88f3-106">Inherits from [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="a88f3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a88f3-107">Properties</span></span>

| <span data-ttu-id="a88f3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a88f3-108">Property</span></span>     | <span data-ttu-id="a88f3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a88f3-109">Type</span></span>        | <span data-ttu-id="a88f3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88f3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a88f3-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="a88f3-111">applicationVersion</span></span>|<span data-ttu-id="a88f3-112">String</span><span class="sxs-lookup"><span data-stu-id="a88f3-112">String</span></span>|<span data-ttu-id="a88f3-113">Identifica a versão do software do aplicativo usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="a88f3-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="a88f3-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="a88f3-114">headerValue</span></span>|<span data-ttu-id="a88f3-115">String</span><span class="sxs-lookup"><span data-stu-id="a88f3-115">String</span></span>|<span data-ttu-id="a88f3-116">Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="a88f3-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="a88f3-117">role</span><span class="sxs-lookup"><span data-stu-id="a88f3-117">role</span></span>|<span data-ttu-id="a88f3-118">String</span><span class="sxs-lookup"><span data-stu-id="a88f3-118">String</span></span>|<span data-ttu-id="a88f3-119">Identifica a função do serviço usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="a88f3-119">Identifies the role of the service used by this endpoint.</span></span> <span data-ttu-id="a88f3-120">Os valores possíveis são: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a88f3-120">Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a88f3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a88f3-121">JSON representation</span></span>

<span data-ttu-id="a88f3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a88f3-122">The following is a JSON representation of the resource.</span></span>

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