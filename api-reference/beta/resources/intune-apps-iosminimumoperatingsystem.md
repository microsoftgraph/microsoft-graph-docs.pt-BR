---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98ad7191b919905e18246e904744b79dfeead06e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161492"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="c6547-103">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c6547-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="c6547-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6547-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6547-106">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="c6547-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="c6547-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6547-107">Properties</span></span>
|<span data-ttu-id="c6547-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6547-108">Property</span></span>|<span data-ttu-id="c6547-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6547-109">Type</span></span>|<span data-ttu-id="c6547-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6547-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6547-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="c6547-111">v8_0</span></span>|<span data-ttu-id="c6547-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6547-112">Boolean</span></span>|<span data-ttu-id="c6547-113">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c6547-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="c6547-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="c6547-114">v9_0</span></span>|<span data-ttu-id="c6547-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6547-115">Boolean</span></span>|<span data-ttu-id="c6547-116">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c6547-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="c6547-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="c6547-117">v10_0</span></span>|<span data-ttu-id="c6547-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6547-118">Boolean</span></span>|<span data-ttu-id="c6547-119">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c6547-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="c6547-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="c6547-120">v11_0</span></span>|<span data-ttu-id="c6547-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6547-121">Boolean</span></span>|<span data-ttu-id="c6547-122">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c6547-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="c6547-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="c6547-123">v12_0</span></span>|<span data-ttu-id="c6547-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6547-124">Boolean</span></span>|<span data-ttu-id="c6547-125">Versão 12,0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c6547-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6547-126">Relações</span><span class="sxs-lookup"><span data-stu-id="c6547-126">Relationships</span></span>
<span data-ttu-id="c6547-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6547-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6547-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6547-128">JSON Representation</span></span>
<span data-ttu-id="c6547-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6547-129">Here is a JSON representation of the resource.</span></span>
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




