---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b0afb706a71ef8e0e3d4877fa7d0df822fe1d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566749"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="ac74c-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="ac74c-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="ac74c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac74c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac74c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac74c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac74c-106">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="ac74c-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="ac74c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac74c-107">Properties</span></span>
|<span data-ttu-id="ac74c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac74c-108">Property</span></span>|<span data-ttu-id="ac74c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac74c-109">Type</span></span>|<span data-ttu-id="ac74c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac74c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac74c-111">description</span><span class="sxs-lookup"><span data-stu-id="ac74c-111">description</span></span>|<span data-ttu-id="ac74c-112">String</span><span class="sxs-lookup"><span data-stu-id="ac74c-112">String</span></span>|<span data-ttu-id="ac74c-113">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="ac74c-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="ac74c-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="ac74c-114">lowestVersion</span></span>|<span data-ttu-id="ac74c-115">String</span><span class="sxs-lookup"><span data-stu-id="ac74c-115">String</span></span>|<span data-ttu-id="ac74c-116">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="ac74c-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="ac74c-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="ac74c-117">highestVersion</span></span>|<span data-ttu-id="ac74c-118">String</span><span class="sxs-lookup"><span data-stu-id="ac74c-118">String</span></span>|<span data-ttu-id="ac74c-119">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="ac74c-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac74c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ac74c-120">Relationships</span></span>
<span data-ttu-id="ac74c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac74c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac74c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac74c-122">JSON Representation</span></span>
<span data-ttu-id="ac74c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac74c-123">Here is a JSON representation of the resource.</span></span>
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





