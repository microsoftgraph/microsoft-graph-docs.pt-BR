---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2ec66c83c13088fb289e271e604154195902ca5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821879"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="d20ee-103">tipo de recurso de excludedApps</span><span class="sxs-lookup"><span data-stu-id="d20ee-103">excludedApps resource type</span></span>

> <span data-ttu-id="d20ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d20ee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d20ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d20ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d20ee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d20ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d20ee-107">Contém propriedades para aplicativos de Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="d20ee-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="d20ee-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d20ee-108">Properties</span></span>
|<span data-ttu-id="d20ee-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d20ee-109">Property</span></span>|<span data-ttu-id="d20ee-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d20ee-110">Type</span></span>|<span data-ttu-id="d20ee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d20ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d20ee-112">acesso</span><span class="sxs-lookup"><span data-stu-id="d20ee-112">access</span></span>|<span data-ttu-id="d20ee-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-113">Boolean</span></span>|<span data-ttu-id="d20ee-114">O valor para se MS Office Access devem ser excluídos ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-115">do Excel</span><span class="sxs-lookup"><span data-stu-id="d20ee-115">excel</span></span>|<span data-ttu-id="d20ee-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-116">Boolean</span></span>|<span data-ttu-id="d20ee-117">O valor para se MS Office Excel devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-118">Groove</span><span class="sxs-lookup"><span data-stu-id="d20ee-118">groove</span></span>|<span data-ttu-id="d20ee-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-119">Boolean</span></span>|<span data-ttu-id="d20ee-120">O valor se OneDrive do MS Office para negócios - Groove devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="d20ee-121">infoPath</span></span>|<span data-ttu-id="d20ee-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-122">Boolean</span></span>|<span data-ttu-id="d20ee-123">O valor para se MS Office InfoPath devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-124">Lync</span><span class="sxs-lookup"><span data-stu-id="d20ee-124">lync</span></span>|<span data-ttu-id="d20ee-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-125">Boolean</span></span>|<span data-ttu-id="d20ee-126">O valor para se Skype do MS Office para negócios - Lync devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="d20ee-127">oneDrive</span></span>|<span data-ttu-id="d20ee-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-128">Boolean</span></span>|<span data-ttu-id="d20ee-129">O valor para se MS Office OneDrive devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="d20ee-130">oneNote</span></span>|<span data-ttu-id="d20ee-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-131">Boolean</span></span>|<span data-ttu-id="d20ee-132">O valor para se MS Office OneNote devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="d20ee-133">outlook</span></span>|<span data-ttu-id="d20ee-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-134">Boolean</span></span>|<span data-ttu-id="d20ee-135">O valor para se MS Office Outlook devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="d20ee-136">powerPoint</span></span>|<span data-ttu-id="d20ee-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-137">Boolean</span></span>|<span data-ttu-id="d20ee-138">O valor para se MS Office PowerPoint devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-139">publisher</span><span class="sxs-lookup"><span data-stu-id="d20ee-139">publisher</span></span>|<span data-ttu-id="d20ee-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-140">Boolean</span></span>|<span data-ttu-id="d20ee-141">O valor para se MS Office Publisher devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="d20ee-142">sharePointDesigner</span></span>|<span data-ttu-id="d20ee-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-143">Boolean</span></span>|<span data-ttu-id="d20ee-144">O valor para se SharePoint Designer do MS Office devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-145">Visio</span><span class="sxs-lookup"><span data-stu-id="d20ee-145">visio</span></span>|<span data-ttu-id="d20ee-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-146">Boolean</span></span>|<span data-ttu-id="d20ee-147">O valor para se MS Office Visio devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="d20ee-148">Word</span><span class="sxs-lookup"><span data-stu-id="d20ee-148">word</span></span>|<span data-ttu-id="d20ee-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="d20ee-149">Boolean</span></span>|<span data-ttu-id="d20ee-150">O valor para se MS Office Word devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="d20ee-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d20ee-151">Relações</span><span class="sxs-lookup"><span data-stu-id="d20ee-151">Relationships</span></span>
<span data-ttu-id="d20ee-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d20ee-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d20ee-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d20ee-153">JSON Representation</span></span>
<span data-ttu-id="d20ee-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d20ee-154">Here is a JSON representation of the resource.</span></span>
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
  "visio": true,
  "word": true
}
```





