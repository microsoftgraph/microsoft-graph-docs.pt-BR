---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395675"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="04e45-103">tipo de recurso de excludedApps</span><span class="sxs-lookup"><span data-stu-id="04e45-103">excludedApps resource type</span></span>

> <span data-ttu-id="04e45-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="04e45-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04e45-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04e45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04e45-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="04e45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e45-107">Contém propriedades para aplicativos de Office365 excluídos.</span><span class="sxs-lookup"><span data-stu-id="04e45-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="04e45-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04e45-108">Properties</span></span>
|<span data-ttu-id="04e45-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04e45-109">Property</span></span>|<span data-ttu-id="04e45-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04e45-110">Type</span></span>|<span data-ttu-id="04e45-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04e45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e45-112">acesso</span><span class="sxs-lookup"><span data-stu-id="04e45-112">access</span></span>|<span data-ttu-id="04e45-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-113">Boolean</span></span>|<span data-ttu-id="04e45-114">O valor para se MS Office Access devem ser excluídos ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-115">do Excel</span><span class="sxs-lookup"><span data-stu-id="04e45-115">excel</span></span>|<span data-ttu-id="04e45-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-116">Boolean</span></span>|<span data-ttu-id="04e45-117">O valor para se MS Office Excel devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-118">Groove</span><span class="sxs-lookup"><span data-stu-id="04e45-118">groove</span></span>|<span data-ttu-id="04e45-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-119">Boolean</span></span>|<span data-ttu-id="04e45-120">O valor se OneDrive do MS Office para negócios - Groove devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="04e45-121">infoPath</span></span>|<span data-ttu-id="04e45-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-122">Boolean</span></span>|<span data-ttu-id="04e45-123">O valor para se MS Office InfoPath devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-124">Lync</span><span class="sxs-lookup"><span data-stu-id="04e45-124">lync</span></span>|<span data-ttu-id="04e45-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-125">Boolean</span></span>|<span data-ttu-id="04e45-126">O valor para se Skype do MS Office para negócios - Lync devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="04e45-127">oneDrive</span></span>|<span data-ttu-id="04e45-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-128">Boolean</span></span>|<span data-ttu-id="04e45-129">O valor para se MS Office OneDrive devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="04e45-130">oneNote</span></span>|<span data-ttu-id="04e45-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-131">Boolean</span></span>|<span data-ttu-id="04e45-132">O valor para se MS Office OneNote devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="04e45-133">outlook</span></span>|<span data-ttu-id="04e45-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-134">Boolean</span></span>|<span data-ttu-id="04e45-135">O valor para se MS Office Outlook devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="04e45-136">powerPoint</span></span>|<span data-ttu-id="04e45-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-137">Boolean</span></span>|<span data-ttu-id="04e45-138">O valor para se MS Office PowerPoint devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-139">publisher</span><span class="sxs-lookup"><span data-stu-id="04e45-139">publisher</span></span>|<span data-ttu-id="04e45-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-140">Boolean</span></span>|<span data-ttu-id="04e45-141">O valor para se MS Office Publisher devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-142">SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="04e45-142">sharePointDesigner</span></span>|<span data-ttu-id="04e45-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-143">Boolean</span></span>|<span data-ttu-id="04e45-144">O valor para se SharePoint Designer do MS Office devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-145">Visio</span><span class="sxs-lookup"><span data-stu-id="04e45-145">visio</span></span>|<span data-ttu-id="04e45-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-146">Boolean</span></span>|<span data-ttu-id="04e45-147">O valor para se MS Office Visio devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="04e45-148">Word</span><span class="sxs-lookup"><span data-stu-id="04e45-148">word</span></span>|<span data-ttu-id="04e45-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e45-149">Boolean</span></span>|<span data-ttu-id="04e45-150">O valor para se MS Office Word devem ser excluído ou não.</span><span class="sxs-lookup"><span data-stu-id="04e45-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04e45-151">Relações</span><span class="sxs-lookup"><span data-stu-id="04e45-151">Relationships</span></span>
<span data-ttu-id="04e45-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04e45-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04e45-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04e45-153">JSON Representation</span></span>
<span data-ttu-id="04e45-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04e45-154">Here is a JSON representation of the resource.</span></span>
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




