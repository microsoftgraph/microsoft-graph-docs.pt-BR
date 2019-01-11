---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7243b337a53cca31054f99ae807e5c17cdd3e372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876263"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="bb2f5-103">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb2f5-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="bb2f5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb2f5-105">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="bb2f5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb2f5-106">Properties</span></span>
|<span data-ttu-id="bb2f5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb2f5-107">Property</span></span>|<span data-ttu-id="bb2f5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb2f5-108">Type</span></span>|<span data-ttu-id="bb2f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb2f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb2f5-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="bb2f5-110">v8_0</span></span>|<span data-ttu-id="bb2f5-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2f5-111">Boolean</span></span>|<span data-ttu-id="bb2f5-112">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="bb2f5-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="bb2f5-113">v9_0</span></span>|<span data-ttu-id="bb2f5-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2f5-114">Boolean</span></span>|<span data-ttu-id="bb2f5-115">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="bb2f5-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="bb2f5-116">v10_0</span></span>|<span data-ttu-id="bb2f5-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2f5-117">Boolean</span></span>|<span data-ttu-id="bb2f5-118">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="bb2f5-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="bb2f5-119">v11_0</span></span>|<span data-ttu-id="bb2f5-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2f5-120">Boolean</span></span>|<span data-ttu-id="bb2f5-121">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="bb2f5-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="bb2f5-122">v12_0</span></span>|<span data-ttu-id="bb2f5-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2f5-123">Boolean</span></span>|<span data-ttu-id="bb2f5-124">Versão 12.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb2f5-125">Relações</span><span class="sxs-lookup"><span data-stu-id="bb2f5-125">Relationships</span></span>
<span data-ttu-id="bb2f5-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb2f5-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb2f5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb2f5-127">JSON Representation</span></span>
<span data-ttu-id="bb2f5-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb2f5-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



