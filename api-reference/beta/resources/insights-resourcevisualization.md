---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e73556061c409f0b22b8ef6bfccd342d20f22c72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021830"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="5444f-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5444f-103">resourceVisualization resource type</span></span>

<span data-ttu-id="5444f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5444f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5444f-105">Tipo complexo que contém as propriedades de [Mysights](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="5444f-105">Complex type containing properties of [itemInsights](iteminsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5444f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5444f-106">JSON representation</span></span>

<span data-ttu-id="5444f-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5444f-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5444f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5444f-108">Properties</span></span>

| <span data-ttu-id="5444f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5444f-109">Property</span></span>              | <span data-ttu-id="5444f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5444f-110">Type</span></span>          | <span data-ttu-id="5444f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5444f-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="5444f-112">title</span><span class="sxs-lookup"><span data-stu-id="5444f-112">title</span></span>                 | <span data-ttu-id="5444f-113">String</span><span class="sxs-lookup"><span data-stu-id="5444f-113">String</span></span>        | <span data-ttu-id="5444f-114">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="5444f-114">The item's title text.</span></span>               |
| <span data-ttu-id="5444f-115">tipo</span><span class="sxs-lookup"><span data-stu-id="5444f-115">type</span></span>              | <span data-ttu-id="5444f-116">String</span><span class="sxs-lookup"><span data-stu-id="5444f-116">String</span></span>        | <span data-ttu-id="5444f-117">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="5444f-117">The item's media type.</span></span> <span data-ttu-id="5444f-118">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="5444f-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="5444f-119">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="5444f-119">See below for supported types.</span></span> |
| <span data-ttu-id="5444f-120">mediaType</span><span class="sxs-lookup"><span data-stu-id="5444f-120">mediaType</span></span>             | <span data-ttu-id="5444f-121">String</span><span class="sxs-lookup"><span data-stu-id="5444f-121">String</span></span>        | <span data-ttu-id="5444f-122">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="5444f-122">The item's media type.</span></span> <span data-ttu-id="5444f-123">Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="5444f-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="5444f-124">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="5444f-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="5444f-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="5444f-125">previewImageUrl</span></span>       | <span data-ttu-id="5444f-126">String</span><span class="sxs-lookup"><span data-stu-id="5444f-126">String</span></span>        | <span data-ttu-id="5444f-127">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="5444f-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="5444f-128">previewText</span><span class="sxs-lookup"><span data-stu-id="5444f-128">previewText</span></span>           | <span data-ttu-id="5444f-129">String</span><span class="sxs-lookup"><span data-stu-id="5444f-129">String</span></span>        | <span data-ttu-id="5444f-130">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="5444f-130">A preview text for the item.</span></span> |
| <span data-ttu-id="5444f-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="5444f-131">containerWebUrl</span></span>       | <span data-ttu-id="5444f-132">String</span><span class="sxs-lookup"><span data-stu-id="5444f-132">String</span></span>        | <span data-ttu-id="5444f-133">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="5444f-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="5444f-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="5444f-134">containerDisplayName</span></span>  | <span data-ttu-id="5444f-135">String</span><span class="sxs-lookup"><span data-stu-id="5444f-135">String</span></span>        | <span data-ttu-id="5444f-136">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="5444f-136">A string describing where the item is stored.</span></span> <span data-ttu-id="5444f-137">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="5444f-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="5444f-138">containerType</span><span class="sxs-lookup"><span data-stu-id="5444f-138">containerType</span></span>         | <span data-ttu-id="5444f-139">String</span><span class="sxs-lookup"><span data-stu-id="5444f-139">String</span></span> | <span data-ttu-id="5444f-140">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="5444f-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="5444f-141">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="5444f-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="5444f-142">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="5444f-142">Type property values</span></span>
-   <span data-ttu-id="5444f-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="5444f-143">PowerPoint</span></span>
-   <span data-ttu-id="5444f-144">Word</span><span class="sxs-lookup"><span data-stu-id="5444f-144">Word</span></span>
-   <span data-ttu-id="5444f-145">Excel</span><span class="sxs-lookup"><span data-stu-id="5444f-145">Excel</span></span>
-   <span data-ttu-id="5444f-146">Documento</span><span class="sxs-lookup"><span data-stu-id="5444f-146">Pdf</span></span>
-   <span data-ttu-id="5444f-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="5444f-147">OneNote</span></span>
-   <span data-ttu-id="5444f-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="5444f-148">OneNotePage</span></span>
-   <span data-ttu-id="5444f-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="5444f-149">InfoPath</span></span>
-   <span data-ttu-id="5444f-150">Visio</span><span class="sxs-lookup"><span data-stu-id="5444f-150">Visio</span></span>
-   <span data-ttu-id="5444f-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="5444f-151">Publisher</span></span>
-   <span data-ttu-id="5444f-152">Project</span><span class="sxs-lookup"><span data-stu-id="5444f-152">Project</span></span>
-   <span data-ttu-id="5444f-153">Access</span><span class="sxs-lookup"><span data-stu-id="5444f-153">Access</span></span>
-   <span data-ttu-id="5444f-154">Email</span><span class="sxs-lookup"><span data-stu-id="5444f-154">Mail</span></span>
-   <span data-ttu-id="5444f-155">Limit</span><span class="sxs-lookup"><span data-stu-id="5444f-155">Csv</span></span>
-   <span data-ttu-id="5444f-156">Arquivar</span><span class="sxs-lookup"><span data-stu-id="5444f-156">Archive</span></span>
-   <span data-ttu-id="5444f-157">XPS</span><span class="sxs-lookup"><span data-stu-id="5444f-157">Xps</span></span>
-   <span data-ttu-id="5444f-158">Áudio</span><span class="sxs-lookup"><span data-stu-id="5444f-158">Audio</span></span>
-   <span data-ttu-id="5444f-159">Vídeo</span><span class="sxs-lookup"><span data-stu-id="5444f-159">Video</span></span>
-   <span data-ttu-id="5444f-160">Imagem</span><span class="sxs-lookup"><span data-stu-id="5444f-160">Image</span></span>
-   <span data-ttu-id="5444f-161">Web</span><span class="sxs-lookup"><span data-stu-id="5444f-161">Web</span></span>
-   <span data-ttu-id="5444f-162">Texto</span><span class="sxs-lookup"><span data-stu-id="5444f-162">Text</span></span>
-   <span data-ttu-id="5444f-163">Xml</span><span class="sxs-lookup"><span data-stu-id="5444f-163">Xml</span></span>
-   <span data-ttu-id="5444f-164">História</span><span class="sxs-lookup"><span data-stu-id="5444f-164">Story</span></span>
-   <span data-ttu-id="5444f-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="5444f-165">ExternalContent</span></span>
-   <span data-ttu-id="5444f-166">Folder</span><span class="sxs-lookup"><span data-stu-id="5444f-166">Folder</span></span>
-   <span data-ttu-id="5444f-167">Outros</span><span class="sxs-lookup"><span data-stu-id="5444f-167">Other</span></span>

<span data-ttu-id="5444f-168">Consulta de exemplo: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="5444f-168">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="5444f-169">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="5444f-169">containerType property values</span></span>
<span data-ttu-id="5444f-170">Os tipos com suporte podem diferir com base nos contêineres dos quais o [Defaultsights](iteminsights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="5444f-170">The supported types can differ based on containers from which [itemInsights](iteminsights.md) returns files.</span></span> <span data-ttu-id="5444f-171">Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="5444f-171">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="5444f-172">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="5444f-172">OneDriveBusiness</span></span>
-   <span data-ttu-id="5444f-173">Site</span><span class="sxs-lookup"><span data-stu-id="5444f-173">Site</span></span>
-   <span data-ttu-id="5444f-174">Email</span><span class="sxs-lookup"><span data-stu-id="5444f-174">Mail</span></span>
-   <span data-ttu-id="5444f-175">DropBox</span><span class="sxs-lookup"><span data-stu-id="5444f-175">DropBox</span></span>
-   <span data-ttu-id="5444f-176">Caixa</span><span class="sxs-lookup"><span data-stu-id="5444f-176">Box</span></span>
-   <span data-ttu-id="5444f-177">GDrive</span><span class="sxs-lookup"><span data-stu-id="5444f-177">GDrive</span></span>

<span data-ttu-id="5444f-178">Consulta de exemplo: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="5444f-178">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>


