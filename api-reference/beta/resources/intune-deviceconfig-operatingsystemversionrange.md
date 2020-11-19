---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9019150efed2f52f884746d7c62f1d7e5a35e83
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293952"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="ce7ba-103">tipo de recurso operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="ce7ba-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="ce7ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce7ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce7ba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce7ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce7ba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce7ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce7ba-107">Intervalo de versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="ce7ba-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="ce7ba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce7ba-108">Properties</span></span>
|<span data-ttu-id="ce7ba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce7ba-109">Property</span></span>|<span data-ttu-id="ce7ba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce7ba-110">Type</span></span>|<span data-ttu-id="ce7ba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce7ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce7ba-112">description</span><span class="sxs-lookup"><span data-stu-id="ce7ba-112">description</span></span>|<span data-ttu-id="ce7ba-113">String</span><span class="sxs-lookup"><span data-stu-id="ce7ba-113">String</span></span>|<span data-ttu-id="ce7ba-114">A descrição desse intervalo (por exemplo, Builds 1702 válidos)</span><span class="sxs-lookup"><span data-stu-id="ce7ba-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="ce7ba-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="ce7ba-115">lowestVersion</span></span>|<span data-ttu-id="ce7ba-116">String</span><span class="sxs-lookup"><span data-stu-id="ce7ba-116">String</span></span>|<span data-ttu-id="ce7ba-117">A versão mais antiga inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="ce7ba-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="ce7ba-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="ce7ba-118">highestVersion</span></span>|<span data-ttu-id="ce7ba-119">String</span><span class="sxs-lookup"><span data-stu-id="ce7ba-119">String</span></span>|<span data-ttu-id="ce7ba-120">A versão mais recente inclusive que este intervalo contém.</span><span class="sxs-lookup"><span data-stu-id="ce7ba-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce7ba-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ce7ba-121">Relationships</span></span>
<span data-ttu-id="ce7ba-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce7ba-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce7ba-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce7ba-123">JSON Representation</span></span>
<span data-ttu-id="ce7ba-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce7ba-124">Here is a JSON representation of the resource.</span></span>
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




