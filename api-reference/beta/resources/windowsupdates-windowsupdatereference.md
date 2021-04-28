---
title: Tipo de recurso windowsUpdateReference
description: Representa o conteúdo Windows 10 de atualização específica.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a75f1afe1c2689760848283bf078b957bb8739ba
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067226"
---
# <a name="windowsupdatereference-resource-type"></a><span data-ttu-id="59a24-103">Tipo de recurso windowsUpdateReference</span><span class="sxs-lookup"><span data-stu-id="59a24-103">windowsUpdateReference resource type</span></span>

<span data-ttu-id="59a24-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="59a24-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59a24-105">Representa o conteúdo Windows 10 de atualização específica.</span><span class="sxs-lookup"><span data-stu-id="59a24-105">Represents specific Windows 10 update content.</span></span>

<span data-ttu-id="59a24-106">Em uma implantação, a mesma Windows de atualização pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.</span><span class="sxs-lookup"><span data-stu-id="59a24-106">In a deployment, the same Windows update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="59a24-107">Todas Windows de atualização existem como um dos seguintes tipos derivados: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) e [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="59a24-107">All Windows update references exist as one of the following derived types: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) and [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span></span>

<span data-ttu-id="59a24-108">Herda de [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="59a24-108">Inherits from [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md).</span></span> <span data-ttu-id="59a24-109">Tipo base [para featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) [e qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="59a24-109">Base type for [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) and [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>

<span data-ttu-id="59a24-110">Esse é um tipo abstrato.</span><span class="sxs-lookup"><span data-stu-id="59a24-110">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="59a24-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59a24-111">Properties</span></span>
<span data-ttu-id="59a24-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="59a24-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="59a24-113">Relações</span><span class="sxs-lookup"><span data-stu-id="59a24-113">Relationships</span></span>
<span data-ttu-id="59a24-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59a24-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59a24-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59a24-115">JSON representation</span></span>
<span data-ttu-id="59a24-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59a24-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsUpdateReference"
}
```

