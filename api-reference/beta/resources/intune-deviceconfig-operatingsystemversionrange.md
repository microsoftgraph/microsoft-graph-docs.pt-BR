---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a5cd426cb4118f1da8e16ce8e097175851204dbb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466396"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="e2e3b-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="e2e3b-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="e2e3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2e3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2e3b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2e3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2e3b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2e3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2e3b-107">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e2e3b-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="e2e3b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2e3b-108">Properties</span></span>
|<span data-ttu-id="e2e3b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2e3b-109">Property</span></span>|<span data-ttu-id="e2e3b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2e3b-110">Type</span></span>|<span data-ttu-id="e2e3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2e3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e3b-112">description</span><span class="sxs-lookup"><span data-stu-id="e2e3b-112">description</span></span>|<span data-ttu-id="e2e3b-113">String</span><span class="sxs-lookup"><span data-stu-id="e2e3b-113">String</span></span>|<span data-ttu-id="e2e3b-114">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="e2e3b-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="e2e3b-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="e2e3b-115">lowestVersion</span></span>|<span data-ttu-id="e2e3b-116">String</span><span class="sxs-lookup"><span data-stu-id="e2e3b-116">String</span></span>|<span data-ttu-id="e2e3b-117">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="e2e3b-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="e2e3b-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="e2e3b-118">highestVersion</span></span>|<span data-ttu-id="e2e3b-119">String</span><span class="sxs-lookup"><span data-stu-id="e2e3b-119">String</span></span>|<span data-ttu-id="e2e3b-120">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="e2e3b-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2e3b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="e2e3b-121">Relationships</span></span>
<span data-ttu-id="e2e3b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2e3b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2e3b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2e3b-123">JSON Representation</span></span>
<span data-ttu-id="e2e3b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2e3b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```



