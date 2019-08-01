---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da56780e66e88baaa074c3106997e3b4a3cc3b64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032344"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="514c0-103">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="514c0-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="514c0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="514c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="514c0-105">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="514c0-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="514c0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="514c0-106">Properties</span></span>
|<span data-ttu-id="514c0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="514c0-107">Property</span></span>|<span data-ttu-id="514c0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="514c0-108">Type</span></span>|<span data-ttu-id="514c0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="514c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="514c0-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="514c0-110">v8_0</span></span>|<span data-ttu-id="514c0-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="514c0-111">Boolean</span></span>|<span data-ttu-id="514c0-112">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="514c0-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="514c0-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="514c0-113">v9_0</span></span>|<span data-ttu-id="514c0-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="514c0-114">Boolean</span></span>|<span data-ttu-id="514c0-115">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="514c0-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="514c0-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="514c0-116">v10_0</span></span>|<span data-ttu-id="514c0-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="514c0-117">Boolean</span></span>|<span data-ttu-id="514c0-118">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="514c0-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="514c0-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="514c0-119">v11_0</span></span>|<span data-ttu-id="514c0-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="514c0-120">Boolean</span></span>|<span data-ttu-id="514c0-121">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="514c0-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="514c0-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="514c0-122">v12_0</span></span>|<span data-ttu-id="514c0-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="514c0-123">Boolean</span></span>|<span data-ttu-id="514c0-124">Versão 12,0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="514c0-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="514c0-125">Relações</span><span class="sxs-lookup"><span data-stu-id="514c0-125">Relationships</span></span>
<span data-ttu-id="514c0-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="514c0-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="514c0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="514c0-127">JSON Representation</span></span>
<span data-ttu-id="514c0-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="514c0-128">Here is a JSON representation of the resource.</span></span>
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



