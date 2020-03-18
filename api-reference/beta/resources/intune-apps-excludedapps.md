---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24813edf732d73905a6b45b9e4fe584b6312a13c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798137"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="6e684-103">tipo de recurso excludedApps</span><span class="sxs-lookup"><span data-stu-id="6e684-103">excludedApps resource type</span></span>

> <span data-ttu-id="6e684-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e684-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e684-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e684-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e684-106">Contém propriedades para aplicativos do Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="6e684-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="6e684-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e684-107">Properties</span></span>
|<span data-ttu-id="6e684-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e684-108">Property</span></span>|<span data-ttu-id="6e684-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e684-109">Type</span></span>|<span data-ttu-id="6e684-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e684-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e684-111">Access</span><span class="sxs-lookup"><span data-stu-id="6e684-111">access</span></span>|<span data-ttu-id="6e684-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-112">Boolean</span></span>|<span data-ttu-id="6e684-113">O valor de se o MS Office Access deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-114">Ele</span><span class="sxs-lookup"><span data-stu-id="6e684-114">excel</span></span>|<span data-ttu-id="6e684-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-115">Boolean</span></span>|<span data-ttu-id="6e684-116">O valor de se o MS Office Excel deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-117">Groove</span><span class="sxs-lookup"><span data-stu-id="6e684-117">groove</span></span>|<span data-ttu-id="6e684-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-118">Boolean</span></span>|<span data-ttu-id="6e684-119">O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-120">Destina</span><span class="sxs-lookup"><span data-stu-id="6e684-120">infoPath</span></span>|<span data-ttu-id="6e684-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-121">Boolean</span></span>|<span data-ttu-id="6e684-122">O valor de se o MS Office InfoPath deve ou não ser excluído.</span><span class="sxs-lookup"><span data-stu-id="6e684-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-123">Lync</span><span class="sxs-lookup"><span data-stu-id="6e684-123">lync</span></span>|<span data-ttu-id="6e684-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-124">Boolean</span></span>|<span data-ttu-id="6e684-125">O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="6e684-126">oneDrive</span></span>|<span data-ttu-id="6e684-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-127">Boolean</span></span>|<span data-ttu-id="6e684-128">O valor de se o MS Office OneDrive deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="6e684-129">oneNote</span></span>|<span data-ttu-id="6e684-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-130">Boolean</span></span>|<span data-ttu-id="6e684-131">O valor de se o MS Office OneNote deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-132">outlook</span><span class="sxs-lookup"><span data-stu-id="6e684-132">outlook</span></span>|<span data-ttu-id="6e684-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-133">Boolean</span></span>|<span data-ttu-id="6e684-134">O valor de se o MS Office Outlook deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-135">Apresentação</span><span class="sxs-lookup"><span data-stu-id="6e684-135">powerPoint</span></span>|<span data-ttu-id="6e684-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-136">Boolean</span></span>|<span data-ttu-id="6e684-137">O valor de se o MS Office PowerPoint deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-138">publicador</span><span class="sxs-lookup"><span data-stu-id="6e684-138">publisher</span></span>|<span data-ttu-id="6e684-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-139">Boolean</span></span>|<span data-ttu-id="6e684-140">O valor de se o MS Office Publisher deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="6e684-141">sharePointDesigner</span></span>|<span data-ttu-id="6e684-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-142">Boolean</span></span>|<span data-ttu-id="6e684-143">O valor de se o MS Office SharePointDesigner deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-144">Teams</span><span class="sxs-lookup"><span data-stu-id="6e684-144">teams</span></span>|<span data-ttu-id="6e684-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-145">Boolean</span></span>|<span data-ttu-id="6e684-146">O valor de se as equipes do MS Office devem ser excluídas ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-147">Visio</span><span class="sxs-lookup"><span data-stu-id="6e684-147">visio</span></span>|<span data-ttu-id="6e684-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-148">Boolean</span></span>|<span data-ttu-id="6e684-149">O valor de se o MS Office Visio deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="6e684-150">palavras</span><span class="sxs-lookup"><span data-stu-id="6e684-150">word</span></span>|<span data-ttu-id="6e684-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e684-151">Boolean</span></span>|<span data-ttu-id="6e684-152">O valor de se o MS Office Word deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="6e684-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e684-153">Relações</span><span class="sxs-lookup"><span data-stu-id="6e684-153">Relationships</span></span>
<span data-ttu-id="6e684-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e684-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e684-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e684-155">JSON Representation</span></span>
<span data-ttu-id="6e684-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e684-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "teams": true,
  "visio": true,
  "word": true
}
```



