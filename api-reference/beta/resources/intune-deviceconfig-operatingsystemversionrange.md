---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20a52b813de13b51fcf94a93fa440337e7123f02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525954"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="a4814-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="a4814-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="a4814-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a4814-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4814-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4814-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4814-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4814-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4814-107">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="a4814-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="a4814-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4814-108">Properties</span></span>
|<span data-ttu-id="a4814-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4814-109">Property</span></span>|<span data-ttu-id="a4814-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4814-110">Type</span></span>|<span data-ttu-id="a4814-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4814-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4814-112">description</span><span class="sxs-lookup"><span data-stu-id="a4814-112">description</span></span>|<span data-ttu-id="a4814-113">String</span><span class="sxs-lookup"><span data-stu-id="a4814-113">String</span></span>|<span data-ttu-id="a4814-114">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="a4814-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="a4814-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="a4814-115">lowestVersion</span></span>|<span data-ttu-id="a4814-116">String</span><span class="sxs-lookup"><span data-stu-id="a4814-116">String</span></span>|<span data-ttu-id="a4814-117">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="a4814-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="a4814-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="a4814-118">highestVersion</span></span>|<span data-ttu-id="a4814-119">String</span><span class="sxs-lookup"><span data-stu-id="a4814-119">String</span></span>|<span data-ttu-id="a4814-120">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="a4814-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4814-121">Relações</span><span class="sxs-lookup"><span data-stu-id="a4814-121">Relationships</span></span>
<span data-ttu-id="a4814-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4814-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4814-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4814-123">JSON Representation</span></span>
<span data-ttu-id="a4814-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4814-124">Here is a JSON representation of the resource.</span></span>
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



