---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
author: tfitzmac
ms.openlocfilehash: b8c9eff985783c953ff099dbf4d5ba00826652c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344622"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="057a8-103">tipo de recurso de excludedApps</span><span class="sxs-lookup"><span data-stu-id="057a8-103">excludedApps resource type</span></span>

> <span data-ttu-id="057a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="057a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="057a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="057a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="057a8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="057a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="057a8-107">Contém propriedades para aplicativos de Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="057a8-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="057a8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="057a8-108">Properties</span></span>
|<span data-ttu-id="057a8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="057a8-109">Property</span></span>|<span data-ttu-id="057a8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="057a8-110">Type</span></span>|<span data-ttu-id="057a8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="057a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="057a8-112">acesso</span><span class="sxs-lookup"><span data-stu-id="057a8-112">access</span></span>|<span data-ttu-id="057a8-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-113">Boolean</span></span>|<span data-ttu-id="057a8-114">O valor para se MS Office Access devem ser excluídos ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-115">do Excel</span><span class="sxs-lookup"><span data-stu-id="057a8-115">excel</span></span>|<span data-ttu-id="057a8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-116">Boolean</span></span>|<span data-ttu-id="057a8-117">O valor para se MS Office Excel devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-118">Groove</span><span class="sxs-lookup"><span data-stu-id="057a8-118">groove</span></span>|<span data-ttu-id="057a8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-119">Boolean</span></span>|<span data-ttu-id="057a8-120">O valor se OneDrive do MS Office para negócios - Groove devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="057a8-121">infoPath</span></span>|<span data-ttu-id="057a8-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-122">Boolean</span></span>|<span data-ttu-id="057a8-123">O valor para se MS Office InfoPath devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-124">Lync</span><span class="sxs-lookup"><span data-stu-id="057a8-124">lync</span></span>|<span data-ttu-id="057a8-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-125">Boolean</span></span>|<span data-ttu-id="057a8-126">O valor para se Skype do MS Office para negócios - Lync devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="057a8-127">oneDrive</span></span>|<span data-ttu-id="057a8-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-128">Boolean</span></span>|<span data-ttu-id="057a8-129">O valor para se MS Office OneDrive devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="057a8-130">oneNote</span></span>|<span data-ttu-id="057a8-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-131">Boolean</span></span>|<span data-ttu-id="057a8-132">O valor para se MS Office OneNote devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="057a8-133">outlook</span></span>|<span data-ttu-id="057a8-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-134">Boolean</span></span>|<span data-ttu-id="057a8-135">O valor para se MS Office Outlook devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="057a8-136">powerPoint</span></span>|<span data-ttu-id="057a8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-137">Boolean</span></span>|<span data-ttu-id="057a8-138">O valor para se MS Office PowerPoint devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-139">publisher</span><span class="sxs-lookup"><span data-stu-id="057a8-139">publisher</span></span>|<span data-ttu-id="057a8-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-140">Boolean</span></span>|<span data-ttu-id="057a8-141">O valor para se MS Office Publisher devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="057a8-142">sharePointDesigner</span></span>|<span data-ttu-id="057a8-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-143">Boolean</span></span>|<span data-ttu-id="057a8-144">O valor para se SharePoint Designer do MS Office devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-145">Visio</span><span class="sxs-lookup"><span data-stu-id="057a8-145">visio</span></span>|<span data-ttu-id="057a8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-146">Boolean</span></span>|<span data-ttu-id="057a8-147">O valor para se MS Office Visio devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="057a8-148">Word</span><span class="sxs-lookup"><span data-stu-id="057a8-148">word</span></span>|<span data-ttu-id="057a8-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="057a8-149">Boolean</span></span>|<span data-ttu-id="057a8-150">O valor para se MS Office Word devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="057a8-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="057a8-151">Relações</span><span class="sxs-lookup"><span data-stu-id="057a8-151">Relationships</span></span>
<span data-ttu-id="057a8-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="057a8-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="057a8-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="057a8-153">JSON Representation</span></span>
<span data-ttu-id="057a8-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="057a8-154">Here is a JSON representation of the resource.</span></span>
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





