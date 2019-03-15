---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dee0d5328f1f69c95159116bf913bc2abb959d7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571687"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="50087-103">tipo de recurso excludedApps</span><span class="sxs-lookup"><span data-stu-id="50087-103">excludedApps resource type</span></span>

> <span data-ttu-id="50087-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50087-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50087-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50087-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50087-106">Contém propriedades para aplicativos do Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="50087-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="50087-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50087-107">Properties</span></span>
|<span data-ttu-id="50087-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50087-108">Property</span></span>|<span data-ttu-id="50087-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="50087-109">Type</span></span>|<span data-ttu-id="50087-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50087-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50087-111">Access</span><span class="sxs-lookup"><span data-stu-id="50087-111">access</span></span>|<span data-ttu-id="50087-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-112">Boolean</span></span>|<span data-ttu-id="50087-113">O valor de se o MS Office Access deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="50087-114">Ele</span><span class="sxs-lookup"><span data-stu-id="50087-114">excel</span></span>|<span data-ttu-id="50087-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-115">Boolean</span></span>|<span data-ttu-id="50087-116">O valor de se o MS Office Excel deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="50087-117">Groove</span><span class="sxs-lookup"><span data-stu-id="50087-117">groove</span></span>|<span data-ttu-id="50087-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-118">Boolean</span></span>|<span data-ttu-id="50087-119">O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="50087-120">Destina</span><span class="sxs-lookup"><span data-stu-id="50087-120">infoPath</span></span>|<span data-ttu-id="50087-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-121">Boolean</span></span>|<span data-ttu-id="50087-122">O valor de se o MS Office InfoPath deve ou não ser excluído.</span><span class="sxs-lookup"><span data-stu-id="50087-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="50087-123">Lync</span><span class="sxs-lookup"><span data-stu-id="50087-123">lync</span></span>|<span data-ttu-id="50087-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-124">Boolean</span></span>|<span data-ttu-id="50087-125">O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="50087-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="50087-126">oneDrive</span></span>|<span data-ttu-id="50087-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-127">Boolean</span></span>|<span data-ttu-id="50087-128">O valor de se o MS Office OneDrive deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="50087-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="50087-129">oneNote</span></span>|<span data-ttu-id="50087-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-130">Boolean</span></span>|<span data-ttu-id="50087-131">O valor de se o MS Office OneNote deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="50087-132">outlook</span><span class="sxs-lookup"><span data-stu-id="50087-132">outlook</span></span>|<span data-ttu-id="50087-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-133">Boolean</span></span>|<span data-ttu-id="50087-134">O valor de se o MS Office Outlook deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="50087-135">Apresentação</span><span class="sxs-lookup"><span data-stu-id="50087-135">powerPoint</span></span>|<span data-ttu-id="50087-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-136">Boolean</span></span>|<span data-ttu-id="50087-137">O valor de se o MS Office PowerPoint deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="50087-138">publicador</span><span class="sxs-lookup"><span data-stu-id="50087-138">publisher</span></span>|<span data-ttu-id="50087-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-139">Boolean</span></span>|<span data-ttu-id="50087-140">O valor de se o MS Office Publisher deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="50087-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="50087-141">sharePointDesigner</span></span>|<span data-ttu-id="50087-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-142">Boolean</span></span>|<span data-ttu-id="50087-143">O valor de se o MS Office SharePointDesigner deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="50087-144">Teams</span><span class="sxs-lookup"><span data-stu-id="50087-144">teams</span></span>|<span data-ttu-id="50087-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-145">Boolean</span></span>|<span data-ttu-id="50087-146">O valor de se as equipes do MS Office devem ser excluídas ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="50087-147">Visio</span><span class="sxs-lookup"><span data-stu-id="50087-147">visio</span></span>|<span data-ttu-id="50087-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-148">Boolean</span></span>|<span data-ttu-id="50087-149">O valor de se o MS Office Visio deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="50087-150">palavras</span><span class="sxs-lookup"><span data-stu-id="50087-150">word</span></span>|<span data-ttu-id="50087-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="50087-151">Boolean</span></span>|<span data-ttu-id="50087-152">O valor de se o MS Office Word deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="50087-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50087-153">Relações</span><span class="sxs-lookup"><span data-stu-id="50087-153">Relationships</span></span>
<span data-ttu-id="50087-154">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="50087-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50087-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50087-155">JSON Representation</span></span>
<span data-ttu-id="50087-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50087-156">Here is a JSON representation of the resource.</span></span>
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




