---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1de8618d20151d079e3f2fdcbadf3658db2b73ef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788419"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="08de7-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="08de7-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="08de7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08de7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08de7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08de7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08de7-106">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="08de7-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="08de7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08de7-107">Properties</span></span>
|<span data-ttu-id="08de7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08de7-108">Property</span></span>|<span data-ttu-id="08de7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="08de7-109">Type</span></span>|<span data-ttu-id="08de7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="08de7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08de7-111">description</span><span class="sxs-lookup"><span data-stu-id="08de7-111">description</span></span>|<span data-ttu-id="08de7-112">String</span><span class="sxs-lookup"><span data-stu-id="08de7-112">String</span></span>|<span data-ttu-id="08de7-113">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="08de7-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="08de7-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="08de7-114">lowestVersion</span></span>|<span data-ttu-id="08de7-115">String</span><span class="sxs-lookup"><span data-stu-id="08de7-115">String</span></span>|<span data-ttu-id="08de7-116">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="08de7-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="08de7-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="08de7-117">highestVersion</span></span>|<span data-ttu-id="08de7-118">String</span><span class="sxs-lookup"><span data-stu-id="08de7-118">String</span></span>|<span data-ttu-id="08de7-119">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="08de7-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08de7-120">Relações</span><span class="sxs-lookup"><span data-stu-id="08de7-120">Relationships</span></span>
<span data-ttu-id="08de7-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08de7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08de7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08de7-122">JSON Representation</span></span>
<span data-ttu-id="08de7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08de7-123">Here is a JSON representation of the resource.</span></span>
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



