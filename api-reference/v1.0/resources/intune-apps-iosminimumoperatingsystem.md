---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
ms.openlocfilehash: 1b39890faf574ab952635c11f113c90479c3ba1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004289"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="99310-103">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99310-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="99310-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="99310-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99310-105">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="99310-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="99310-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99310-106">Properties</span></span>
|<span data-ttu-id="99310-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99310-107">Property</span></span>|<span data-ttu-id="99310-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="99310-108">Type</span></span>|<span data-ttu-id="99310-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="99310-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99310-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="99310-110">v8_0</span></span>|<span data-ttu-id="99310-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="99310-111">Boolean</span></span>|<span data-ttu-id="99310-112">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="99310-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="99310-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="99310-113">v9_0</span></span>|<span data-ttu-id="99310-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="99310-114">Boolean</span></span>|<span data-ttu-id="99310-115">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="99310-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="99310-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="99310-116">v10_0</span></span>|<span data-ttu-id="99310-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="99310-117">Boolean</span></span>|<span data-ttu-id="99310-118">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="99310-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="99310-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="99310-119">v11_0</span></span>|<span data-ttu-id="99310-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="99310-120">Boolean</span></span>|<span data-ttu-id="99310-121">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="99310-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="99310-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="99310-122">v12_0</span></span>|<span data-ttu-id="99310-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="99310-123">Boolean</span></span>|<span data-ttu-id="99310-124">Versão 12.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="99310-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99310-125">Relações</span><span class="sxs-lookup"><span data-stu-id="99310-125">Relationships</span></span>
<span data-ttu-id="99310-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99310-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99310-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99310-127">JSON Representation</span></span>
<span data-ttu-id="99310-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99310-128">Here is a JSON representation of the resource.</span></span>
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



