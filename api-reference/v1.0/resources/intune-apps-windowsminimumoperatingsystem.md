---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571706"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="7471e-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7471e-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="7471e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7471e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7471e-105">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="7471e-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="7471e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7471e-106">Properties</span></span>
|<span data-ttu-id="7471e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7471e-107">Property</span></span>|<span data-ttu-id="7471e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7471e-108">Type</span></span>|<span data-ttu-id="7471e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7471e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7471e-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="7471e-110">v8_0</span></span>|<span data-ttu-id="7471e-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="7471e-111">Boolean</span></span>|<span data-ttu-id="7471e-112">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="7471e-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="7471e-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="7471e-113">v8_1</span></span>|<span data-ttu-id="7471e-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="7471e-114">Boolean</span></span>|<span data-ttu-id="7471e-115">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="7471e-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="7471e-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="7471e-116">v10_0</span></span>|<span data-ttu-id="7471e-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="7471e-117">Boolean</span></span>|<span data-ttu-id="7471e-118">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="7471e-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7471e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7471e-119">Relationships</span></span>
<span data-ttu-id="7471e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7471e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7471e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7471e-121">JSON Representation</span></span>
<span data-ttu-id="7471e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7471e-122">Here is a JSON representation of the resource.</span></span>
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



