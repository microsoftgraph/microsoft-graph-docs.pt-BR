---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91418a1a60a87f381dc15c63a60d69e8c264a5c3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991244"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c437d-103">tipo de recurso excludedApps</span><span class="sxs-lookup"><span data-stu-id="c437d-103">excludedApps resource type</span></span>

> <span data-ttu-id="c437d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c437d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c437d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c437d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c437d-106">Contém propriedades para aplicativos do Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="c437d-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="c437d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c437d-107">Properties</span></span>
|<span data-ttu-id="c437d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c437d-108">Property</span></span>|<span data-ttu-id="c437d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c437d-109">Type</span></span>|<span data-ttu-id="c437d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c437d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c437d-111">Access</span><span class="sxs-lookup"><span data-stu-id="c437d-111">access</span></span>|<span data-ttu-id="c437d-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-112">Boolean</span></span>|<span data-ttu-id="c437d-113">O valor de se o MS Office Access deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-114">Ele</span><span class="sxs-lookup"><span data-stu-id="c437d-114">excel</span></span>|<span data-ttu-id="c437d-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-115">Boolean</span></span>|<span data-ttu-id="c437d-116">O valor de se o MS Office Excel deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-117">Groove</span><span class="sxs-lookup"><span data-stu-id="c437d-117">groove</span></span>|<span data-ttu-id="c437d-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-118">Boolean</span></span>|<span data-ttu-id="c437d-119">O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-120">Destina</span><span class="sxs-lookup"><span data-stu-id="c437d-120">infoPath</span></span>|<span data-ttu-id="c437d-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-121">Boolean</span></span>|<span data-ttu-id="c437d-122">O valor de se o MS Office InfoPath deve ou não ser excluído.</span><span class="sxs-lookup"><span data-stu-id="c437d-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-123">Lync</span><span class="sxs-lookup"><span data-stu-id="c437d-123">lync</span></span>|<span data-ttu-id="c437d-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-124">Boolean</span></span>|<span data-ttu-id="c437d-125">O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="c437d-126">oneDrive</span></span>|<span data-ttu-id="c437d-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-127">Boolean</span></span>|<span data-ttu-id="c437d-128">O valor de se o MS Office OneDrive deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="c437d-129">oneNote</span></span>|<span data-ttu-id="c437d-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-130">Boolean</span></span>|<span data-ttu-id="c437d-131">O valor de se o MS Office OneNote deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-132">outlook</span><span class="sxs-lookup"><span data-stu-id="c437d-132">outlook</span></span>|<span data-ttu-id="c437d-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-133">Boolean</span></span>|<span data-ttu-id="c437d-134">O valor de se o MS Office Outlook deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-135">Apresentação</span><span class="sxs-lookup"><span data-stu-id="c437d-135">powerPoint</span></span>|<span data-ttu-id="c437d-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-136">Boolean</span></span>|<span data-ttu-id="c437d-137">O valor de se o MS Office PowerPoint deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-138">publicador</span><span class="sxs-lookup"><span data-stu-id="c437d-138">publisher</span></span>|<span data-ttu-id="c437d-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-139">Boolean</span></span>|<span data-ttu-id="c437d-140">O valor de se o MS Office Publisher deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="c437d-141">sharePointDesigner</span></span>|<span data-ttu-id="c437d-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-142">Boolean</span></span>|<span data-ttu-id="c437d-143">O valor de se o MS Office SharePointDesigner deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-144">Teams</span><span class="sxs-lookup"><span data-stu-id="c437d-144">teams</span></span>|<span data-ttu-id="c437d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-145">Boolean</span></span>|<span data-ttu-id="c437d-146">O valor de se as equipes do MS Office devem ser excluídas ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-147">Visio</span><span class="sxs-lookup"><span data-stu-id="c437d-147">visio</span></span>|<span data-ttu-id="c437d-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-148">Boolean</span></span>|<span data-ttu-id="c437d-149">O valor de se o MS Office Visio deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c437d-150">palavras</span><span class="sxs-lookup"><span data-stu-id="c437d-150">word</span></span>|<span data-ttu-id="c437d-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="c437d-151">Boolean</span></span>|<span data-ttu-id="c437d-152">O valor de se o MS Office Word deve ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="c437d-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c437d-153">Relações</span><span class="sxs-lookup"><span data-stu-id="c437d-153">Relationships</span></span>
<span data-ttu-id="c437d-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c437d-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c437d-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c437d-155">JSON Representation</span></span>
<span data-ttu-id="c437d-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c437d-156">Here is a JSON representation of the resource.</span></span>
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





