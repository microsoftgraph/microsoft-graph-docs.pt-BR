---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 521b82448d58a831f88bdf9d548612aee86bcba6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972947"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="eace5-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eace5-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="eace5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eace5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eace5-105">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="eace5-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="eace5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eace5-106">Properties</span></span>
|<span data-ttu-id="eace5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eace5-107">Property</span></span>|<span data-ttu-id="eace5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eace5-108">Type</span></span>|<span data-ttu-id="eace5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eace5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eace5-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="eace5-110">v8_0</span></span>|<span data-ttu-id="eace5-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="eace5-111">Boolean</span></span>|<span data-ttu-id="eace5-112">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="eace5-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="eace5-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="eace5-113">v8_1</span></span>|<span data-ttu-id="eace5-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="eace5-114">Boolean</span></span>|<span data-ttu-id="eace5-115">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="eace5-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="eace5-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="eace5-116">v10_0</span></span>|<span data-ttu-id="eace5-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="eace5-117">Boolean</span></span>|<span data-ttu-id="eace5-118">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="eace5-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eace5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="eace5-119">Relationships</span></span>
<span data-ttu-id="eace5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eace5-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eace5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eace5-121">JSON Representation</span></span>
<span data-ttu-id="eace5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eace5-122">Here is a JSON representation of the resource.</span></span>
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



