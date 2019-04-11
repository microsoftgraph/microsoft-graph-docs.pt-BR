---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b0afb706a71ef8e0e3d4877fa7d0df822fe1d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788118"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="ead07-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="ead07-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="ead07-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ead07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ead07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ead07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ead07-106">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="ead07-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="ead07-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ead07-107">Properties</span></span>
|<span data-ttu-id="ead07-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ead07-108">Property</span></span>|<span data-ttu-id="ead07-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ead07-109">Type</span></span>|<span data-ttu-id="ead07-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ead07-111">description</span><span class="sxs-lookup"><span data-stu-id="ead07-111">description</span></span>|<span data-ttu-id="ead07-112">String</span><span class="sxs-lookup"><span data-stu-id="ead07-112">String</span></span>|<span data-ttu-id="ead07-113">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="ead07-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="ead07-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="ead07-114">lowestVersion</span></span>|<span data-ttu-id="ead07-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ead07-115">String</span></span>|<span data-ttu-id="ead07-116">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="ead07-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="ead07-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="ead07-117">highestVersion</span></span>|<span data-ttu-id="ead07-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ead07-118">String</span></span>|<span data-ttu-id="ead07-119">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="ead07-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ead07-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ead07-120">Relationships</span></span>
<span data-ttu-id="ead07-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ead07-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ead07-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ead07-122">JSON Representation</span></span>
<span data-ttu-id="ead07-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ead07-123">Here is a JSON representation of the resource.</span></span>
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





