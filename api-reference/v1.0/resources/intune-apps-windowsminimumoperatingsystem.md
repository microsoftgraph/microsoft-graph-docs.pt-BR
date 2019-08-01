---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a92d02f6994a7cd18ba44c7da5b43768e87fc61a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032071"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="aa3ff-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="aa3ff-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="aa3ff-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa3ff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa3ff-105">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="aa3ff-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="aa3ff-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa3ff-106">Properties</span></span>
|<span data-ttu-id="aa3ff-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa3ff-107">Property</span></span>|<span data-ttu-id="aa3ff-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa3ff-108">Type</span></span>|<span data-ttu-id="aa3ff-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa3ff-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa3ff-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="aa3ff-110">v8_0</span></span>|<span data-ttu-id="aa3ff-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa3ff-111">Boolean</span></span>|<span data-ttu-id="aa3ff-112">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="aa3ff-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="aa3ff-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="aa3ff-113">v8_1</span></span>|<span data-ttu-id="aa3ff-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa3ff-114">Boolean</span></span>|<span data-ttu-id="aa3ff-115">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="aa3ff-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="aa3ff-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="aa3ff-116">v10_0</span></span>|<span data-ttu-id="aa3ff-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa3ff-117">Boolean</span></span>|<span data-ttu-id="aa3ff-118">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="aa3ff-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa3ff-119">Relações</span><span class="sxs-lookup"><span data-stu-id="aa3ff-119">Relationships</span></span>
<span data-ttu-id="aa3ff-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa3ff-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa3ff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa3ff-121">JSON Representation</span></span>
<span data-ttu-id="aa3ff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa3ff-122">Here is a JSON representation of the resource.</span></span>
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



