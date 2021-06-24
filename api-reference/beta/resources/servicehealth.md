---
title: Tipo de recurso serviceHealth
description: Representa as informações de saúde de um serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c11750bbffe64315c6263a26d7dbab333f42b7cf
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109067"
---
# <a name="servicehealth-resource-type"></a><span data-ttu-id="73573-103">Tipo de recurso serviceHealth</span><span class="sxs-lookup"><span data-stu-id="73573-103">serviceHealth resource type</span></span>

<span data-ttu-id="73573-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73573-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73573-105">Representa as informações de saúde de um serviço.</span><span class="sxs-lookup"><span data-stu-id="73573-105">Represents the health information of a service.</span></span>

## <a name="methods"></a><span data-ttu-id="73573-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="73573-106">Methods</span></span>
|<span data-ttu-id="73573-107">Método</span><span class="sxs-lookup"><span data-stu-id="73573-107">Method</span></span>|<span data-ttu-id="73573-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73573-108">Return type</span></span>|<span data-ttu-id="73573-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73573-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73573-110">Obter serviceHealth</span><span class="sxs-lookup"><span data-stu-id="73573-110">Get serviceHealth</span></span>](../api/servicehealth-get.md)|[<span data-ttu-id="73573-111">serviceHealth</span><span class="sxs-lookup"><span data-stu-id="73573-111">serviceHealth</span></span>](../resources/servicehealth.md)|<span data-ttu-id="73573-112">Recupere as propriedades e as relações de um [objeto serviceHealth.](../resources/servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="73573-112">Retrieve the properties and relationships of a [serviceHealth](../resources/servicehealth.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73573-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73573-113">Properties</span></span>
|<span data-ttu-id="73573-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73573-114">Property</span></span>|<span data-ttu-id="73573-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="73573-115">Type</span></span>|<span data-ttu-id="73573-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="73573-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73573-117">id</span><span class="sxs-lookup"><span data-stu-id="73573-117">id</span></span>|<span data-ttu-id="73573-118">String</span><span class="sxs-lookup"><span data-stu-id="73573-118">String</span></span>|<span data-ttu-id="73573-119">A ID do serviço.</span><span class="sxs-lookup"><span data-stu-id="73573-119">The service id.</span></span>|
|<span data-ttu-id="73573-120">service</span><span class="sxs-lookup"><span data-stu-id="73573-120">service</span></span>|<span data-ttu-id="73573-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73573-121">String</span></span>|<span data-ttu-id="73573-122">O nome do serviço.</span><span class="sxs-lookup"><span data-stu-id="73573-122">The service name.</span></span>|
|<span data-ttu-id="73573-123">status</span><span class="sxs-lookup"><span data-stu-id="73573-123">status</span></span>|<span data-ttu-id="73573-124">serviceHealthStatus</span><span class="sxs-lookup"><span data-stu-id="73573-124">serviceHealthStatus</span></span>|<span data-ttu-id="73573-125">Mostrar o status de saúde do serviço overral.</span><span class="sxs-lookup"><span data-stu-id="73573-125">Show the overral service health status.</span></span> <span data-ttu-id="73573-126">Os valores possíveis são: `serviceOperational` , , , , , , , , `investigating` , , , `restoringService` , , `verifyingService` , , , `serviceRestored` , , `postIncidentReviewPublished` `serviceDegradation` , `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` . `reported` `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="73573-126">Possible values are: `serviceOperational`, `investigating`, `restoringService`, `verifyingService`, `serviceRestored`, `postIncidentReviewPublished`, `serviceDegradation`, `serviceInterruption`, `extendedRecovery`, `falsePositive`, `investigationSuspended`, `resolved`, `mitigatedExternal`, `mitigated`, `resolvedExternal`, `confirmed`, `reported`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73573-127">Relações</span><span class="sxs-lookup"><span data-stu-id="73573-127">Relationships</span></span>
|<span data-ttu-id="73573-128">Relação</span><span class="sxs-lookup"><span data-stu-id="73573-128">Relationship</span></span>|<span data-ttu-id="73573-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="73573-129">Type</span></span>|<span data-ttu-id="73573-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="73573-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73573-131">issues</span><span class="sxs-lookup"><span data-stu-id="73573-131">issues</span></span>|<span data-ttu-id="73573-132">Collection([serviceHealthIssue](../resources/servicehealthissue.md))</span><span class="sxs-lookup"><span data-stu-id="73573-132">Collection([serviceHealthIssue](../resources/servicehealthissue.md))</span></span>|<span data-ttu-id="73573-133">Uma coleção de problemas aconteceu no serviço, com informações detalhadas para cada problema.</span><span class="sxs-lookup"><span data-stu-id="73573-133">A collection of issues happened on the service, with detailed information for each issue.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73573-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73573-134">JSON representation</span></span>
<span data-ttu-id="73573-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73573-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealth",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String",
  "id": "String (identifier)"
}
```

