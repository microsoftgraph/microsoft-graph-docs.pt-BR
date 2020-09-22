---
title: tipo de recurso teleconferenceDeviceQuality
description: Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 455a69257e880c71c28fa7968e5e8294075437e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086274"
---
# <a name="teleconferencedevicequality-resource-type"></a><span data-ttu-id="d522d-103">tipo de recurso teleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="d522d-103">teleconferenceDeviceQuality resource type</span></span>

<span data-ttu-id="d522d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d522d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d522d-105">Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="d522d-105">Represents video teleconferencing device session-level quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="d522d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d522d-106">Properties</span></span>

| <span data-ttu-id="d522d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d522d-107">Property</span></span>     | <span data-ttu-id="d522d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d522d-108">Type</span></span>        | <span data-ttu-id="d522d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d522d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d522d-110">callChainId</span><span class="sxs-lookup"><span data-stu-id="d522d-110">callChainId</span></span>|<span data-ttu-id="d522d-111">Guid</span><span class="sxs-lookup"><span data-stu-id="d522d-111">Guid</span></span>|<span data-ttu-id="d522d-112">Um identificador exclusivo para todas as chamadas de participantes em uma conferência ou um identificador exclusivo para duas chamadas de participantes na chamada P2P.</span><span class="sxs-lookup"><span data-stu-id="d522d-112">A unique identifier for all  the participant calls in a conference or a unique identifier for two participant calls in P2P call.</span></span> <span data-ttu-id="d522d-113">Isso precisa ser copiado de `Microsoft.Graph.Call.CallChainId`.</span><span class="sxs-lookup"><span data-stu-id="d522d-113">This needs to be copied over from `Microsoft.Graph.Call.CallChainId`.</span></span>|
|<span data-ttu-id="d522d-114">cloudServiceDeploymentEnvironment</span><span class="sxs-lookup"><span data-stu-id="d522d-114">cloudServiceDeploymentEnvironment</span></span>|<span data-ttu-id="d522d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d522d-115">String</span></span>|<span data-ttu-id="d522d-116">Uma região geográfica onde o serviço é implantado, como `ProdNoam` .</span><span class="sxs-lookup"><span data-stu-id="d522d-116">A geo-region where the service is deployed, such as `ProdNoam`.</span></span>|
|<span data-ttu-id="d522d-117">cloudServiceDeploymentId</span><span class="sxs-lookup"><span data-stu-id="d522d-117">cloudServiceDeploymentId</span></span>|<span data-ttu-id="d522d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d522d-118">String</span></span>|<span data-ttu-id="d522d-119">Um identificador de implantação exclusivo atribuído pelo Azure.</span><span class="sxs-lookup"><span data-stu-id="d522d-119">A unique deployment identifier assigned by Azure.</span></span>|
|<span data-ttu-id="d522d-120">cloudServiceInstanceName</span><span class="sxs-lookup"><span data-stu-id="d522d-120">cloudServiceInstanceName</span></span>|<span data-ttu-id="d522d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d522d-121">String</span></span>|<span data-ttu-id="d522d-122">O nome da instância do serviço de nuvem implantada do Azure, como `FrontEnd_IN_3` .</span><span class="sxs-lookup"><span data-stu-id="d522d-122">The Azure deployed cloud service instance name, such as `FrontEnd_IN_3`.</span></span>|
|<span data-ttu-id="d522d-123">cloudServiceName</span><span class="sxs-lookup"><span data-stu-id="d522d-123">cloudServiceName</span></span>|<span data-ttu-id="d522d-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d522d-124">String</span></span>|<span data-ttu-id="d522d-125">O nome do serviço de nuvem implantada do Azure, como `contoso.cloudapp.net` .</span><span class="sxs-lookup"><span data-stu-id="d522d-125">The Azure deployed cloud service name, such as `contoso.cloudapp.net`.</span></span>|
|<span data-ttu-id="d522d-126">deviceDescription</span><span class="sxs-lookup"><span data-stu-id="d522d-126">deviceDescription</span></span>|<span data-ttu-id="d522d-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d522d-127">String</span></span>|<span data-ttu-id="d522d-128">Qualquer descrição adicional, como `VTC Bldg 30/21` .</span><span class="sxs-lookup"><span data-stu-id="d522d-128">Any additional description, such as `VTC Bldg 30/21`.</span></span>|
|<span data-ttu-id="d522d-129">deviceName</span><span class="sxs-lookup"><span data-stu-id="d522d-129">deviceName</span></span>|<span data-ttu-id="d522d-130">String</span><span class="sxs-lookup"><span data-stu-id="d522d-130">String</span></span>|<span data-ttu-id="d522d-131">O nome do agente de mídia do usuário, como `Cisco SX80` .</span><span class="sxs-lookup"><span data-stu-id="d522d-131">The user media agent name, such as `Cisco SX80`.</span></span>|
|<span data-ttu-id="d522d-132">mediaLegId</span><span class="sxs-lookup"><span data-stu-id="d522d-132">mediaLegId</span></span>|<span data-ttu-id="d522d-133">Guid</span><span class="sxs-lookup"><span data-stu-id="d522d-133">Guid</span></span>|<span data-ttu-id="d522d-134">Um identificador exclusivo para um trecho de mídia específico de um participante de uma conferência.</span><span class="sxs-lookup"><span data-stu-id="d522d-134">A unique identifier for a specific media leg of a participant in a conference.</span></span>  <span data-ttu-id="d522d-135">Um participante pode ter vários identificadores de trechos de mídia se o redirecionamento ocorrer.</span><span class="sxs-lookup"><span data-stu-id="d522d-135">One participant can have multiple media leg identifiers if retargeting happens.</span></span> <span data-ttu-id="d522d-136">O parceiro CVI atribui esse valor.</span><span class="sxs-lookup"><span data-stu-id="d522d-136">CVI partner assigns this value.</span></span>|
|<span data-ttu-id="d522d-137">mediaQualityList</span><span class="sxs-lookup"><span data-stu-id="d522d-137">mediaQualityList</span></span>|<span data-ttu-id="d522d-138">coleção [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)</span><span class="sxs-lookup"><span data-stu-id="d522d-138">[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md) collection</span></span>|<span data-ttu-id="d522d-139">A lista de qualidades de mídia em uma sessão de mídia (chamada), como qualidade de áudio, qualidade de vídeo e/ou qualidade de compartilhamento de tela.</span><span class="sxs-lookup"><span data-stu-id="d522d-139">The list of media qualities in a media session (call), such as audio quality, video quality, and/or screen sharing quality.</span></span>|
|<span data-ttu-id="d522d-140">participante de participantes</span><span class="sxs-lookup"><span data-stu-id="d522d-140">participantId</span></span>|<span data-ttu-id="d522d-141">Guid</span><span class="sxs-lookup"><span data-stu-id="d522d-141">Guid</span></span>|<span data-ttu-id="d522d-142">Um identificador exclusivo para um participante específico em uma conferência.</span><span class="sxs-lookup"><span data-stu-id="d522d-142">A unique identifier for a specific participant in a conference.</span></span> <span data-ttu-id="d522d-143">O parceiro CVI precisa copiar `Call.MyParticipantId` para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="d522d-143">The CVI partner needs to copy over `Call.MyParticipantId` to this property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d522d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d522d-144">JSON representation</span></span>

<span data-ttu-id="d522d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d522d-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
  "baseType": null
}-->

```json
{
  "callChainId": "Guid",
  "cloudServiceDeploymentEnvironment": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceName": "String",
  "deviceDescription": "String",
  "deviceName": "String",
  "mediaLegId": "Guid",
  "mediaQualityList": [{"@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"}],
  "participantId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

