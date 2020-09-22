---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30aaecee77c4cdea7539e790fd1204ecd9e8dc98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003931"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="e92a5-103">tipo de recurso excludedApps</span><span class="sxs-lookup"><span data-stu-id="e92a5-103">excludedApps resource type</span></span>

<span data-ttu-id="e92a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e92a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e92a5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e92a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e92a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e92a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e92a5-107">Contém propriedades para aplicativos do Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="e92a5-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="e92a5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e92a5-108">Properties</span></span>
|<span data-ttu-id="e92a5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e92a5-109">Property</span></span>|<span data-ttu-id="e92a5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e92a5-110">Type</span></span>|<span data-ttu-id="e92a5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e92a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e92a5-112">Access</span><span class="sxs-lookup"><span data-stu-id="e92a5-112">access</span></span>|<span data-ttu-id="e92a5-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-113">Boolean</span></span>|<span data-ttu-id="e92a5-114">O valor de se o MS Office Access deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-115">Bing</span><span class="sxs-lookup"><span data-stu-id="e92a5-115">bing</span></span>|<span data-ttu-id="e92a5-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-116">Boolean</span></span>|<span data-ttu-id="e92a5-117">O valor da pesquisa da Microsoft como padrão deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-117">The value for if Microsoft Search as default should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-118">Ele</span><span class="sxs-lookup"><span data-stu-id="e92a5-118">excel</span></span>|<span data-ttu-id="e92a5-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-119">Boolean</span></span>|<span data-ttu-id="e92a5-120">O valor de se o MS Office Excel deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-120">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-121">Groove</span><span class="sxs-lookup"><span data-stu-id="e92a5-121">groove</span></span>|<span data-ttu-id="e92a5-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-122">Boolean</span></span>|<span data-ttu-id="e92a5-123">O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-123">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-124">Destina</span><span class="sxs-lookup"><span data-stu-id="e92a5-124">infoPath</span></span>|<span data-ttu-id="e92a5-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-125">Boolean</span></span>|<span data-ttu-id="e92a5-126">O valor de se o MS Office InfoPath deve ou não ser excluído.</span><span class="sxs-lookup"><span data-stu-id="e92a5-126">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-127">Lync</span><span class="sxs-lookup"><span data-stu-id="e92a5-127">lync</span></span>|<span data-ttu-id="e92a5-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-128">Boolean</span></span>|<span data-ttu-id="e92a5-129">O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-129">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-130">oneDrive</span><span class="sxs-lookup"><span data-stu-id="e92a5-130">oneDrive</span></span>|<span data-ttu-id="e92a5-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-131">Boolean</span></span>|<span data-ttu-id="e92a5-132">O valor de se o MS Office OneDrive deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-132">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-133">oneNote</span><span class="sxs-lookup"><span data-stu-id="e92a5-133">oneNote</span></span>|<span data-ttu-id="e92a5-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-134">Boolean</span></span>|<span data-ttu-id="e92a5-135">O valor de se o MS Office OneNote deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-135">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-136">outlook</span><span class="sxs-lookup"><span data-stu-id="e92a5-136">outlook</span></span>|<span data-ttu-id="e92a5-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-137">Boolean</span></span>|<span data-ttu-id="e92a5-138">O valor de se o MS Office Outlook deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-138">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-139">Apresentação</span><span class="sxs-lookup"><span data-stu-id="e92a5-139">powerPoint</span></span>|<span data-ttu-id="e92a5-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-140">Boolean</span></span>|<span data-ttu-id="e92a5-141">O valor de se o MS Office PowerPoint deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-141">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-142">publicador</span><span class="sxs-lookup"><span data-stu-id="e92a5-142">publisher</span></span>|<span data-ttu-id="e92a5-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-143">Boolean</span></span>|<span data-ttu-id="e92a5-144">O valor de se o MS Office Publisher deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-144">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-145">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="e92a5-145">sharePointDesigner</span></span>|<span data-ttu-id="e92a5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-146">Boolean</span></span>|<span data-ttu-id="e92a5-147">O valor de se o MS Office SharePointDesigner deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-147">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-148">Teams</span><span class="sxs-lookup"><span data-stu-id="e92a5-148">teams</span></span>|<span data-ttu-id="e92a5-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-149">Boolean</span></span>|<span data-ttu-id="e92a5-150">O valor de se as equipes do MS Office devem ser excluídas ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-150">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-151">Visio</span><span class="sxs-lookup"><span data-stu-id="e92a5-151">visio</span></span>|<span data-ttu-id="e92a5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-152">Boolean</span></span>|<span data-ttu-id="e92a5-153">O valor de se o MS Office Visio deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-153">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="e92a5-154">palavras</span><span class="sxs-lookup"><span data-stu-id="e92a5-154">word</span></span>|<span data-ttu-id="e92a5-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92a5-155">Boolean</span></span>|<span data-ttu-id="e92a5-156">O valor de se o MS Office Word deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="e92a5-156">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e92a5-157">Relações</span><span class="sxs-lookup"><span data-stu-id="e92a5-157">Relationships</span></span>
<span data-ttu-id="e92a5-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e92a5-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e92a5-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e92a5-159">JSON Representation</span></span>
<span data-ttu-id="e92a5-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e92a5-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "bing": true,
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






