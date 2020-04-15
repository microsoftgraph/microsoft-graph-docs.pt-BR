---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd61874b0b7149c718ba790b2cdee23912a0a832
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439582"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="289ec-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="289ec-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="289ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="289ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="289ec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="289ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="289ec-106">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="289ec-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="289ec-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="289ec-107">Properties</span></span>
|<span data-ttu-id="289ec-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="289ec-108">Property</span></span>|<span data-ttu-id="289ec-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="289ec-109">Type</span></span>|<span data-ttu-id="289ec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="289ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="289ec-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="289ec-111">v8_0</span></span>|<span data-ttu-id="289ec-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="289ec-112">Boolean</span></span>|<span data-ttu-id="289ec-113">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="289ec-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="289ec-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="289ec-114">v8_1</span></span>|<span data-ttu-id="289ec-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="289ec-115">Boolean</span></span>|<span data-ttu-id="289ec-116">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="289ec-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="289ec-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="289ec-117">v10_0</span></span>|<span data-ttu-id="289ec-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="289ec-118">Boolean</span></span>|<span data-ttu-id="289ec-119">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="289ec-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="289ec-120">Relações</span><span class="sxs-lookup"><span data-stu-id="289ec-120">Relationships</span></span>
<span data-ttu-id="289ec-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="289ec-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="289ec-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="289ec-122">JSON Representation</span></span>
<span data-ttu-id="289ec-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="289ec-123">Here is a JSON representation of the resource.</span></span>
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







