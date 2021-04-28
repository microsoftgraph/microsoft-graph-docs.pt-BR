---
title: Tipo de recurso expeditedQualityUpdateReference
description: Representa Windows 10 conteúdo de atualização de qualidade para acelerar.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 685f65d8c5661cd4c8308ed712ab3fddedbae51d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067815"
---
# <a name="expeditedqualityupdatereference-resource-type"></a><span data-ttu-id="1ac94-103">Tipo de recurso expeditedQualityUpdateReference</span><span class="sxs-lookup"><span data-stu-id="1ac94-103">expeditedQualityUpdateReference resource type</span></span>

<span data-ttu-id="1ac94-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="1ac94-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ac94-105">Representa Windows 10 conteúdo de atualização de qualidade para acelerar.</span><span class="sxs-lookup"><span data-stu-id="1ac94-105">Represents Windows 10 quality update content to expedite.</span></span>

<span data-ttu-id="1ac94-106">Em uma implantação, a mesma referência de atualização de qualidade acelerada pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.</span><span class="sxs-lookup"><span data-stu-id="1ac94-106">In a deployment, the same expedited quality update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="1ac94-107">Herda [de qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="1ac94-107">Inherits from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1ac94-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ac94-108">Properties</span></span>
|<span data-ttu-id="1ac94-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ac94-109">Property</span></span>|<span data-ttu-id="1ac94-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ac94-110">Type</span></span>|<span data-ttu-id="1ac94-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ac94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ac94-112">classificação</span><span class="sxs-lookup"><span data-stu-id="1ac94-112">classification</span></span>|<span data-ttu-id="1ac94-113">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="1ac94-113">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="1ac94-114">Especifica a classificação do conteúdo referenciado.</span><span class="sxs-lookup"><span data-stu-id="1ac94-114">Specifies the classification of the referenced content.</span></span> <span data-ttu-id="1ac94-115">Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**.</span><span class="sxs-lookup"><span data-stu-id="1ac94-115">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="1ac94-116">O valor padrão é `security`.</span><span class="sxs-lookup"><span data-stu-id="1ac94-116">Default value is `security`.</span></span> <span data-ttu-id="1ac94-117">Os valores possíveis são: `security` .</span><span class="sxs-lookup"><span data-stu-id="1ac94-117">Possible values are: `security`.</span></span> <span data-ttu-id="1ac94-118">Herdado [de qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="1ac94-118">Inherited from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>|
|<span data-ttu-id="1ac94-119">equivalentContent</span><span class="sxs-lookup"><span data-stu-id="1ac94-119">equivalentContent</span></span>|<span data-ttu-id="1ac94-120">microsoft.graph.windowsUpdates.equivalentContentOption</span><span class="sxs-lookup"><span data-stu-id="1ac94-120">microsoft.graph.windowsUpdates.equivalentContentOption</span></span>|<span data-ttu-id="1ac94-121">Especifica outro conteúdo a ser considerado como equivalente.</span><span class="sxs-lookup"><span data-stu-id="1ac94-121">Specifies other content to consider as equivalent.</span></span> <span data-ttu-id="1ac94-122">Oferece suporte a um subconjunto dos valores **para equivalentContentOption**.</span><span class="sxs-lookup"><span data-stu-id="1ac94-122">Supports a subset of the values for **equivalentContentOption**.</span></span> <span data-ttu-id="1ac94-123">O valor padrão é `latestSecurity`.</span><span class="sxs-lookup"><span data-stu-id="1ac94-123">Default value is `latestSecurity`.</span></span> <span data-ttu-id="1ac94-124">Os valores possíveis são: `latestSecurity` .</span><span class="sxs-lookup"><span data-stu-id="1ac94-124">Possible values are: `latestSecurity`.</span></span>|
|<span data-ttu-id="1ac94-125">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1ac94-125">releaseDateTime</span></span>|<span data-ttu-id="1ac94-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ac94-126">DateTimeOffset</span></span>|<span data-ttu-id="1ac94-127">Especifica uma atualização de qualidade com a **classificação** determinada por sua data de publicação (ou seja, a última atualização publicada na data especificada).</span><span class="sxs-lookup"><span data-stu-id="1ac94-127">Specifies a quality update with the given **classification** by its publish date (i.e. the last update published on the specified date).</span></span> <span data-ttu-id="1ac94-128">Todos os dispositivos com uma atualização publicada antes da **versãoDateTime** receberão uma atualização de qualidade acelerada.</span><span class="sxs-lookup"><span data-stu-id="1ac94-128">Any devices with an update that was published prior to the **releaseDateTime** will receive an expedited quality update.</span></span> <span data-ttu-id="1ac94-129">Herdado [de qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="1ac94-129">Inherited from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ac94-130">Relações</span><span class="sxs-lookup"><span data-stu-id="1ac94-130">Relationships</span></span>
<span data-ttu-id="1ac94-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ac94-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ac94-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ac94-132">JSON representation</span></span>
<span data-ttu-id="1ac94-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ac94-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)",
  "equivalentContent": "String"
}
```

