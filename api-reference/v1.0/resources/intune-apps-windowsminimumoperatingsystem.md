---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: tfitzmac
ms.openlocfilehash: ea1953bd0d58d4e578ffb7171fc157166072189b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314725"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="ff952-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff952-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="ff952-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ff952-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff952-105">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="ff952-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="ff952-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff952-106">Properties</span></span>
|<span data-ttu-id="ff952-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff952-107">Property</span></span>|<span data-ttu-id="ff952-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff952-108">Type</span></span>|<span data-ttu-id="ff952-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff952-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff952-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="ff952-110">v8_0</span></span>|<span data-ttu-id="ff952-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff952-111">Boolean</span></span>|<span data-ttu-id="ff952-112">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="ff952-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="ff952-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="ff952-113">v8_1</span></span>|<span data-ttu-id="ff952-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff952-114">Boolean</span></span>|<span data-ttu-id="ff952-115">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="ff952-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="ff952-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="ff952-116">v10_0</span></span>|<span data-ttu-id="ff952-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff952-117">Boolean</span></span>|<span data-ttu-id="ff952-118">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="ff952-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff952-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ff952-119">Relationships</span></span>
<span data-ttu-id="ff952-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff952-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff952-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff952-121">JSON Representation</span></span>
<span data-ttu-id="ff952-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff952-122">Here is a JSON representation of the resource.</span></span>
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



