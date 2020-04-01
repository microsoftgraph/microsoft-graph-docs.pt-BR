---
title: tipo de recurso teleconferenceDeviceQuality
description: Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c96382644793b57dd0eaa7b0f95213897e6068ce
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082707"
---
# <a name="teleconferencedevicequality-resource-type"></a><span data-ttu-id="09d95-103">tipo de recurso teleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="09d95-103">teleconferenceDeviceQuality resource type</span></span>

<span data-ttu-id="09d95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d95-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09d95-105">Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="09d95-105">Represents video teleconferencing device session-level quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="09d95-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09d95-106">Properties</span></span>

| <span data-ttu-id="09d95-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09d95-107">Property</span></span>     | <span data-ttu-id="09d95-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d95-108">Type</span></span>        | <span data-ttu-id="09d95-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d95-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09d95-110">callChainId</span><span class="sxs-lookup"><span data-stu-id="09d95-110">callChainId</span></span>|<span data-ttu-id="09d95-111">Guid</span><span class="sxs-lookup"><span data-stu-id="09d95-111">Guid</span></span>|<span data-ttu-id="09d95-112">Um identificador exclusivo para todas as chamadas de participantes em uma conferência ou um identificador exclusivo para duas chamadas de participantes na chamada P2P.</span><span class="sxs-lookup"><span data-stu-id="09d95-112">A unique identifier for all  the participant calls in a conference or a unique identifier for two participant calls in P2P call.</span></span> <span data-ttu-id="09d95-113">Isso precisa ser copiado de `Microsoft.Graph.Call.CallChainId`.</span><span class="sxs-lookup"><span data-stu-id="09d95-113">This needs to be copied over from `Microsoft.Graph.Call.CallChainId`.</span></span>|
|<span data-ttu-id="09d95-114">cloudServiceDeploymentEnvironment</span><span class="sxs-lookup"><span data-stu-id="09d95-114">cloudServiceDeploymentEnvironment</span></span>|<span data-ttu-id="09d95-115">String</span><span class="sxs-lookup"><span data-stu-id="09d95-115">String</span></span>|<span data-ttu-id="09d95-116">Uma região geográfica onde o serviço é implantado, como `ProdNoam`.</span><span class="sxs-lookup"><span data-stu-id="09d95-116">A geo-region where the service is deployed, such as `ProdNoam`.</span></span>|
|<span data-ttu-id="09d95-117">cloudServiceDeploymentId</span><span class="sxs-lookup"><span data-stu-id="09d95-117">cloudServiceDeploymentId</span></span>|<span data-ttu-id="09d95-118">String</span><span class="sxs-lookup"><span data-stu-id="09d95-118">String</span></span>|<span data-ttu-id="09d95-119">Um identificador de implantação exclusivo atribuído pelo Azure.</span><span class="sxs-lookup"><span data-stu-id="09d95-119">A unique deployment identifier assigned by Azure.</span></span>|
|<span data-ttu-id="09d95-120">cloudServiceInstanceName</span><span class="sxs-lookup"><span data-stu-id="09d95-120">cloudServiceInstanceName</span></span>|<span data-ttu-id="09d95-121">String</span><span class="sxs-lookup"><span data-stu-id="09d95-121">String</span></span>|<span data-ttu-id="09d95-122">O nome da instância do serviço de nuvem implantada do Azure, como `FrontEnd_IN_3`.</span><span class="sxs-lookup"><span data-stu-id="09d95-122">The Azure deployed cloud service instance name, such as `FrontEnd_IN_3`.</span></span>|
|<span data-ttu-id="09d95-123">cloudServiceName</span><span class="sxs-lookup"><span data-stu-id="09d95-123">cloudServiceName</span></span>|<span data-ttu-id="09d95-124">String</span><span class="sxs-lookup"><span data-stu-id="09d95-124">String</span></span>|<span data-ttu-id="09d95-125">O nome do serviço de nuvem implantada `contoso.cloudapp.net`do Azure, como.</span><span class="sxs-lookup"><span data-stu-id="09d95-125">The Azure deployed cloud service name, such as `contoso.cloudapp.net`.</span></span>|
|<span data-ttu-id="09d95-126">deviceDescription</span><span class="sxs-lookup"><span data-stu-id="09d95-126">deviceDescription</span></span>|<span data-ttu-id="09d95-127">String</span><span class="sxs-lookup"><span data-stu-id="09d95-127">String</span></span>|<span data-ttu-id="09d95-128">Qualquer descrição adicional, como `VTC Bldg 30/21`.</span><span class="sxs-lookup"><span data-stu-id="09d95-128">Any additional description, such as `VTC Bldg 30/21`.</span></span>|
|<span data-ttu-id="09d95-129">deviceName</span><span class="sxs-lookup"><span data-stu-id="09d95-129">deviceName</span></span>|<span data-ttu-id="09d95-130">String</span><span class="sxs-lookup"><span data-stu-id="09d95-130">String</span></span>|<span data-ttu-id="09d95-131">O nome do agente de mídia do usuário `Cisco SX80`, como.</span><span class="sxs-lookup"><span data-stu-id="09d95-131">The user media agent name, such as `Cisco SX80`.</span></span>|
|<span data-ttu-id="09d95-132">mediaLegId</span><span class="sxs-lookup"><span data-stu-id="09d95-132">mediaLegId</span></span>|<span data-ttu-id="09d95-133">Guid</span><span class="sxs-lookup"><span data-stu-id="09d95-133">Guid</span></span>|<span data-ttu-id="09d95-134">Um identificador exclusivo para um trecho de mídia específico de um participante de uma conferência.</span><span class="sxs-lookup"><span data-stu-id="09d95-134">A unique identifier for a specific media leg of a participant in a conference.</span></span>  <span data-ttu-id="09d95-135">Um participante pode ter vários identificadores de trechos de mídia se o redirecionamento ocorrer.</span><span class="sxs-lookup"><span data-stu-id="09d95-135">One participant can have multiple media leg identifiers if retargeting happens.</span></span> <span data-ttu-id="09d95-136">O parceiro CVI atribui esse valor.</span><span class="sxs-lookup"><span data-stu-id="09d95-136">CVI partner assigns this value.</span></span>|
|<span data-ttu-id="09d95-137">mediaQualityList</span><span class="sxs-lookup"><span data-stu-id="09d95-137">mediaQualityList</span></span>|<span data-ttu-id="09d95-138">coleção [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)</span><span class="sxs-lookup"><span data-stu-id="09d95-138">[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md) collection</span></span>|<span data-ttu-id="09d95-139">A lista de qualidades de mídia em uma sessão de mídia (chamada), como qualidade de áudio, qualidade de vídeo e/ou qualidade de compartilhamento de tela.</span><span class="sxs-lookup"><span data-stu-id="09d95-139">The list of media qualities in a media session (call), such as audio quality, video quality, and/or screen sharing quality.</span></span>|
|<span data-ttu-id="09d95-140">participante de participantes</span><span class="sxs-lookup"><span data-stu-id="09d95-140">participantId</span></span>|<span data-ttu-id="09d95-141">Guid</span><span class="sxs-lookup"><span data-stu-id="09d95-141">Guid</span></span>|<span data-ttu-id="09d95-142">Um identificador exclusivo para um participante específico em uma conferência.</span><span class="sxs-lookup"><span data-stu-id="09d95-142">A unique identifier for a specific participant in a conference.</span></span> <span data-ttu-id="09d95-143">O parceiro CVI precisa copiar `Call.MyParticipantId` para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="09d95-143">The CVI partner needs to copy over `Call.MyParticipantId` to this property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09d95-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09d95-144">JSON representation</span></span>

<span data-ttu-id="09d95-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09d95-145">The following is a JSON representation of the resource.</span></span>

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
