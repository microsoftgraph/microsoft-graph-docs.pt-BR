---
title: Tipo de recurso windowsMinimumOperatingSystem
description: O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 574ca504ec7b0cd736735323e534bfd3ed17f31b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755977"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="90671-103">Tipo de recurso windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="90671-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="90671-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90671-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90671-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90671-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90671-106">O sistema operacional mínimo obrigatório para um aplicativo móvel do Windows.</span><span class="sxs-lookup"><span data-stu-id="90671-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="90671-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90671-107">Properties</span></span>
|<span data-ttu-id="90671-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90671-108">Property</span></span>|<span data-ttu-id="90671-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="90671-109">Type</span></span>|<span data-ttu-id="90671-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="90671-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90671-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="90671-111">v8_0</span></span>|<span data-ttu-id="90671-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="90671-112">Boolean</span></span>|<span data-ttu-id="90671-113">Windows 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="90671-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="90671-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="90671-114">v8_1</span></span>|<span data-ttu-id="90671-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="90671-115">Boolean</span></span>|<span data-ttu-id="90671-116">Windows 8.1 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="90671-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="90671-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="90671-117">v10_0</span></span>|<span data-ttu-id="90671-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="90671-118">Boolean</span></span>|<span data-ttu-id="90671-119">Windows 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="90671-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90671-120">Relações</span><span class="sxs-lookup"><span data-stu-id="90671-120">Relationships</span></span>
<span data-ttu-id="90671-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="90671-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90671-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90671-122">JSON Representation</span></span>
<span data-ttu-id="90671-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90671-123">Here is a JSON representation of the resource.</span></span>
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




