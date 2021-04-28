---
title: Tipo de recurso softwareUpdateReference
description: Representa conteúdo de atualização específico.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 66f7f895bd3d7556ad5e3d35066236663b474f41
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067824"
---
# <a name="softwareupdatereference-resource-type"></a><span data-ttu-id="587f8-103">Tipo de recurso softwareUpdateReference</span><span class="sxs-lookup"><span data-stu-id="587f8-103">softwareUpdateReference resource type</span></span>

<span data-ttu-id="587f8-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="587f8-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="587f8-105">Representa conteúdo de atualização específico.</span><span class="sxs-lookup"><span data-stu-id="587f8-105">Represents specific update content.</span></span>

<span data-ttu-id="587f8-106">Em uma implantação, o mesmo **softwareUpdateReference** pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextualmente equivalente para todos os dispositivos na implantação.</span><span class="sxs-lookup"><span data-stu-id="587f8-106">In a deployment, the same **softwareUpdateReference** could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="587f8-107">Todas as referências de atualização de software existem como um dos seguintes tipos derivados: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="587f8-107">All software update references exist as one of the following derived types: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).</span></span>

<span data-ttu-id="587f8-108">Herda de [deployableContent](../resources/windowsupdates-deployablecontent.md).</span><span class="sxs-lookup"><span data-stu-id="587f8-108">Inherits from [deployableContent](../resources/windowsupdates-deployablecontent.md).</span></span> <span data-ttu-id="587f8-109">Tipo base [para windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="587f8-109">Base type for [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span>

<span data-ttu-id="587f8-110">Esse é um tipo abstrato.</span><span class="sxs-lookup"><span data-stu-id="587f8-110">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="587f8-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="587f8-111">Properties</span></span>
<span data-ttu-id="587f8-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="587f8-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="587f8-113">Relações</span><span class="sxs-lookup"><span data-stu-id="587f8-113">Relationships</span></span>
<span data-ttu-id="587f8-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="587f8-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="587f8-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="587f8-115">JSON representation</span></span>
<span data-ttu-id="587f8-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="587f8-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateReference"
}
```

