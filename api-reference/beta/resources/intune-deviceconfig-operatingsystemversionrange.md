---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521f7d0b0ec4ddab728ed3b95c27acf21695b0d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148605"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="6d3c9-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="6d3c9-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="6d3c9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d3c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d3c9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d3c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d3c9-106">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="6d3c9-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="6d3c9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d3c9-107">Properties</span></span>
|<span data-ttu-id="6d3c9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d3c9-108">Property</span></span>|<span data-ttu-id="6d3c9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3c9-109">Type</span></span>|<span data-ttu-id="6d3c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d3c9-111">description</span><span class="sxs-lookup"><span data-stu-id="6d3c9-111">description</span></span>|<span data-ttu-id="6d3c9-112">String</span><span class="sxs-lookup"><span data-stu-id="6d3c9-112">String</span></span>|<span data-ttu-id="6d3c9-113">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="6d3c9-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="6d3c9-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="6d3c9-114">lowestVersion</span></span>|<span data-ttu-id="6d3c9-115">String</span><span class="sxs-lookup"><span data-stu-id="6d3c9-115">String</span></span>|<span data-ttu-id="6d3c9-116">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="6d3c9-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="6d3c9-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="6d3c9-117">highestVersion</span></span>|<span data-ttu-id="6d3c9-118">String</span><span class="sxs-lookup"><span data-stu-id="6d3c9-118">String</span></span>|<span data-ttu-id="6d3c9-119">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="6d3c9-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d3c9-120">Relações</span><span class="sxs-lookup"><span data-stu-id="6d3c9-120">Relationships</span></span>
<span data-ttu-id="6d3c9-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d3c9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d3c9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d3c9-122">JSON Representation</span></span>
<span data-ttu-id="6d3c9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d3c9-123">Here is a JSON representation of the resource.</span></span>
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




