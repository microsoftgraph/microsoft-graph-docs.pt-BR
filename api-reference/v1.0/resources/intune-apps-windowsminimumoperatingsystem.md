---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254461"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="72529-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="72529-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="72529-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72529-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72529-105">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="72529-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="72529-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72529-106">Properties</span></span>
|<span data-ttu-id="72529-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72529-107">Property</span></span>|<span data-ttu-id="72529-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="72529-108">Type</span></span>|<span data-ttu-id="72529-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="72529-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72529-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="72529-110">v8_0</span></span>|<span data-ttu-id="72529-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="72529-111">Boolean</span></span>|<span data-ttu-id="72529-112">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="72529-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="72529-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="72529-113">v8_1</span></span>|<span data-ttu-id="72529-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="72529-114">Boolean</span></span>|<span data-ttu-id="72529-115">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="72529-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="72529-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="72529-116">v10_0</span></span>|<span data-ttu-id="72529-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="72529-117">Boolean</span></span>|<span data-ttu-id="72529-118">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="72529-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72529-119">Relações</span><span class="sxs-lookup"><span data-stu-id="72529-119">Relationships</span></span>
<span data-ttu-id="72529-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72529-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72529-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72529-121">JSON Representation</span></span>
<span data-ttu-id="72529-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72529-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



