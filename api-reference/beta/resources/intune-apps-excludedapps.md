---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92a86a9b875caf47d5c06145716642bb3d6a7e81
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790898"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="7dc7f-103">tipo de recurso excludedApps</span><span class="sxs-lookup"><span data-stu-id="7dc7f-103">excludedApps resource type</span></span>

<span data-ttu-id="7dc7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dc7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dc7f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dc7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dc7f-107">Contém propriedades para aplicativos do Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="7dc7f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dc7f-108">Properties</span></span>
|<span data-ttu-id="7dc7f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dc7f-109">Property</span></span>|<span data-ttu-id="7dc7f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dc7f-110">Type</span></span>|<span data-ttu-id="7dc7f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dc7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dc7f-112">Access</span><span class="sxs-lookup"><span data-stu-id="7dc7f-112">access</span></span>|<span data-ttu-id="7dc7f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-113">Boolean</span></span>|<span data-ttu-id="7dc7f-114">O valor de se o MS Office Access deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-115">Bing</span><span class="sxs-lookup"><span data-stu-id="7dc7f-115">bing</span></span>|<span data-ttu-id="7dc7f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-116">Boolean</span></span>|<span data-ttu-id="7dc7f-117">O valor da pesquisa da Microsoft como padrão deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-117">The value for if Microsoft Search as default should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-118">Ele</span><span class="sxs-lookup"><span data-stu-id="7dc7f-118">excel</span></span>|<span data-ttu-id="7dc7f-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-119">Boolean</span></span>|<span data-ttu-id="7dc7f-120">O valor de se o MS Office Excel deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-120">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-121">Groove</span><span class="sxs-lookup"><span data-stu-id="7dc7f-121">groove</span></span>|<span data-ttu-id="7dc7f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-122">Boolean</span></span>|<span data-ttu-id="7dc7f-123">O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-123">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-124">Destina</span><span class="sxs-lookup"><span data-stu-id="7dc7f-124">infoPath</span></span>|<span data-ttu-id="7dc7f-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-125">Boolean</span></span>|<span data-ttu-id="7dc7f-126">O valor de se o MS Office InfoPath deve ou não ser excluído.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-126">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-127">Lync</span><span class="sxs-lookup"><span data-stu-id="7dc7f-127">lync</span></span>|<span data-ttu-id="7dc7f-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-128">Boolean</span></span>|<span data-ttu-id="7dc7f-129">O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-129">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-130">oneDrive</span><span class="sxs-lookup"><span data-stu-id="7dc7f-130">oneDrive</span></span>|<span data-ttu-id="7dc7f-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-131">Boolean</span></span>|<span data-ttu-id="7dc7f-132">O valor de se o MS Office OneDrive deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-132">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-133">oneNote</span><span class="sxs-lookup"><span data-stu-id="7dc7f-133">oneNote</span></span>|<span data-ttu-id="7dc7f-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-134">Boolean</span></span>|<span data-ttu-id="7dc7f-135">O valor de se o MS Office OneNote deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-135">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-136">outlook</span><span class="sxs-lookup"><span data-stu-id="7dc7f-136">outlook</span></span>|<span data-ttu-id="7dc7f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-137">Boolean</span></span>|<span data-ttu-id="7dc7f-138">O valor de se o MS Office Outlook deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-138">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-139">Apresentação</span><span class="sxs-lookup"><span data-stu-id="7dc7f-139">powerPoint</span></span>|<span data-ttu-id="7dc7f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-140">Boolean</span></span>|<span data-ttu-id="7dc7f-141">O valor de se o MS Office PowerPoint deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-141">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-142">publicador</span><span class="sxs-lookup"><span data-stu-id="7dc7f-142">publisher</span></span>|<span data-ttu-id="7dc7f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-143">Boolean</span></span>|<span data-ttu-id="7dc7f-144">O valor de se o MS Office Publisher deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-144">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-145">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="7dc7f-145">sharePointDesigner</span></span>|<span data-ttu-id="7dc7f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-146">Boolean</span></span>|<span data-ttu-id="7dc7f-147">O valor de se o MS Office SharePointDesigner deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-147">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-148">Teams</span><span class="sxs-lookup"><span data-stu-id="7dc7f-148">teams</span></span>|<span data-ttu-id="7dc7f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-149">Boolean</span></span>|<span data-ttu-id="7dc7f-150">O valor de se as equipes do MS Office devem ser excluídas ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-150">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-151">Visio</span><span class="sxs-lookup"><span data-stu-id="7dc7f-151">visio</span></span>|<span data-ttu-id="7dc7f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-152">Boolean</span></span>|<span data-ttu-id="7dc7f-153">O valor de se o MS Office Visio deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-153">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="7dc7f-154">palavras</span><span class="sxs-lookup"><span data-stu-id="7dc7f-154">word</span></span>|<span data-ttu-id="7dc7f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc7f-155">Boolean</span></span>|<span data-ttu-id="7dc7f-156">O valor de se o MS Office Word deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-156">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dc7f-157">Relações</span><span class="sxs-lookup"><span data-stu-id="7dc7f-157">Relationships</span></span>
<span data-ttu-id="7dc7f-158">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7dc7f-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dc7f-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dc7f-159">JSON Representation</span></span>
<span data-ttu-id="7dc7f-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7dc7f-160">Here is a JSON representation of the resource.</span></span>
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



