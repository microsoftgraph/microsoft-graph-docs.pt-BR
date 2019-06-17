---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a123c645262986711dbe28cc170443f948d2f5c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987898"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="7fd0c-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="7fd0c-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="7fd0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7fd0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fd0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7fd0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fd0c-106">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="7fd0c-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="7fd0c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fd0c-107">Properties</span></span>
|<span data-ttu-id="7fd0c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fd0c-108">Property</span></span>|<span data-ttu-id="7fd0c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fd0c-109">Type</span></span>|<span data-ttu-id="7fd0c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fd0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fd0c-111">description</span><span class="sxs-lookup"><span data-stu-id="7fd0c-111">description</span></span>|<span data-ttu-id="7fd0c-112">String</span><span class="sxs-lookup"><span data-stu-id="7fd0c-112">String</span></span>|<span data-ttu-id="7fd0c-113">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="7fd0c-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="7fd0c-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="7fd0c-114">lowestVersion</span></span>|<span data-ttu-id="7fd0c-115">String</span><span class="sxs-lookup"><span data-stu-id="7fd0c-115">String</span></span>|<span data-ttu-id="7fd0c-116">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="7fd0c-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="7fd0c-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="7fd0c-117">highestVersion</span></span>|<span data-ttu-id="7fd0c-118">String</span><span class="sxs-lookup"><span data-stu-id="7fd0c-118">String</span></span>|<span data-ttu-id="7fd0c-119">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="7fd0c-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fd0c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7fd0c-120">Relationships</span></span>
<span data-ttu-id="7fd0c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fd0c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fd0c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fd0c-122">JSON Representation</span></span>
<span data-ttu-id="7fd0c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fd0c-123">Here is a JSON representation of the resource.</span></span>
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





