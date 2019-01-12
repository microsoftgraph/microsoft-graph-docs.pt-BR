---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943946"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="bf6bf-103">tipo de recurso de excludedApps</span><span class="sxs-lookup"><span data-stu-id="bf6bf-103">excludedApps resource type</span></span>

> <span data-ttu-id="bf6bf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf6bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf6bf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf6bf-107">Contém propriedades para aplicativos de Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="bf6bf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf6bf-108">Properties</span></span>
|<span data-ttu-id="bf6bf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf6bf-109">Property</span></span>|<span data-ttu-id="bf6bf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf6bf-110">Type</span></span>|<span data-ttu-id="bf6bf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf6bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf6bf-112">acesso</span><span class="sxs-lookup"><span data-stu-id="bf6bf-112">access</span></span>|<span data-ttu-id="bf6bf-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-113">Boolean</span></span>|<span data-ttu-id="bf6bf-114">O valor para se MS Office Access devem ser excluídos ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-115">do Excel</span><span class="sxs-lookup"><span data-stu-id="bf6bf-115">excel</span></span>|<span data-ttu-id="bf6bf-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-116">Boolean</span></span>|<span data-ttu-id="bf6bf-117">O valor para se MS Office Excel devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-118">Groove</span><span class="sxs-lookup"><span data-stu-id="bf6bf-118">groove</span></span>|<span data-ttu-id="bf6bf-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-119">Boolean</span></span>|<span data-ttu-id="bf6bf-120">O valor se OneDrive do MS Office para negócios - Groove devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="bf6bf-121">infoPath</span></span>|<span data-ttu-id="bf6bf-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-122">Boolean</span></span>|<span data-ttu-id="bf6bf-123">O valor para se MS Office InfoPath devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-124">Lync</span><span class="sxs-lookup"><span data-stu-id="bf6bf-124">lync</span></span>|<span data-ttu-id="bf6bf-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-125">Boolean</span></span>|<span data-ttu-id="bf6bf-126">O valor para se Skype do MS Office para negócios - Lync devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="bf6bf-127">oneDrive</span></span>|<span data-ttu-id="bf6bf-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-128">Boolean</span></span>|<span data-ttu-id="bf6bf-129">O valor para se MS Office OneDrive devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="bf6bf-130">oneNote</span></span>|<span data-ttu-id="bf6bf-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-131">Boolean</span></span>|<span data-ttu-id="bf6bf-132">O valor para se MS Office OneNote devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="bf6bf-133">outlook</span></span>|<span data-ttu-id="bf6bf-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-134">Boolean</span></span>|<span data-ttu-id="bf6bf-135">O valor para se MS Office Outlook devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="bf6bf-136">powerPoint</span></span>|<span data-ttu-id="bf6bf-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-137">Boolean</span></span>|<span data-ttu-id="bf6bf-138">O valor para se MS Office PowerPoint devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-139">publisher</span><span class="sxs-lookup"><span data-stu-id="bf6bf-139">publisher</span></span>|<span data-ttu-id="bf6bf-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-140">Boolean</span></span>|<span data-ttu-id="bf6bf-141">O valor para se MS Office Publisher devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="bf6bf-142">sharePointDesigner</span></span>|<span data-ttu-id="bf6bf-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-143">Boolean</span></span>|<span data-ttu-id="bf6bf-144">O valor para se SharePoint Designer do MS Office devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-145">Visio</span><span class="sxs-lookup"><span data-stu-id="bf6bf-145">visio</span></span>|<span data-ttu-id="bf6bf-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-146">Boolean</span></span>|<span data-ttu-id="bf6bf-147">O valor para se MS Office Visio devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="bf6bf-148">Word</span><span class="sxs-lookup"><span data-stu-id="bf6bf-148">word</span></span>|<span data-ttu-id="bf6bf-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6bf-149">Boolean</span></span>|<span data-ttu-id="bf6bf-150">O valor para se MS Office Word devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf6bf-151">Relações</span><span class="sxs-lookup"><span data-stu-id="bf6bf-151">Relationships</span></span>
<span data-ttu-id="bf6bf-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf6bf-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf6bf-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf6bf-153">JSON Representation</span></span>
<span data-ttu-id="bf6bf-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf6bf-154">Here is a JSON representation of the resource.</span></span>
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





