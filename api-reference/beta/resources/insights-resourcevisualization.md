---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: b49ce2c0fb0c1d2ab167ffbb033bf11b0171a20f
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844488"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="e5426-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="e5426-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5426-104">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="e5426-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5426-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5426-105">JSON representation</span></span>

<span data-ttu-id="e5426-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e5426-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e5426-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5426-107">Properties</span></span>

| <span data-ttu-id="e5426-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5426-108">Property</span></span>              | <span data-ttu-id="e5426-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5426-109">Type</span></span>          | <span data-ttu-id="e5426-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5426-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="e5426-111">title</span><span class="sxs-lookup"><span data-stu-id="e5426-111">title</span></span>                 | <span data-ttu-id="e5426-112">String</span><span class="sxs-lookup"><span data-stu-id="e5426-112">String</span></span>        | <span data-ttu-id="e5426-113">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="e5426-113">The item's title text.</span></span>               |
| <span data-ttu-id="e5426-114">type</span><span class="sxs-lookup"><span data-stu-id="e5426-114">type</span></span>              | <span data-ttu-id="e5426-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5426-115">String</span></span>        | <span data-ttu-id="e5426-116">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="e5426-116">The item's media type.</span></span> <span data-ttu-id="e5426-117">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="e5426-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="e5426-118">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="e5426-118">See below for supported types.</span></span> |
| <span data-ttu-id="e5426-119">Mídia</span><span class="sxs-lookup"><span data-stu-id="e5426-119">mediaType</span></span>             | <span data-ttu-id="e5426-120">String</span><span class="sxs-lookup"><span data-stu-id="e5426-120">String</span></span>        | <span data-ttu-id="e5426-121">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="e5426-121">The item's media type.</span></span> <span data-ttu-id="e5426-122">Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="e5426-122">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="e5426-123">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="e5426-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="e5426-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="e5426-124">previewImageUrl</span></span>       | <span data-ttu-id="e5426-125">String</span><span class="sxs-lookup"><span data-stu-id="e5426-125">String</span></span>        | <span data-ttu-id="e5426-126">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="e5426-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="e5426-127">previewText</span><span class="sxs-lookup"><span data-stu-id="e5426-127">previewText</span></span>           | <span data-ttu-id="e5426-128">String</span><span class="sxs-lookup"><span data-stu-id="e5426-128">String</span></span>        | <span data-ttu-id="e5426-129">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="e5426-129">A preview text for the item.</span></span> |
| <span data-ttu-id="e5426-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="e5426-130">containerWebUrl</span></span>       | <span data-ttu-id="e5426-131">String</span><span class="sxs-lookup"><span data-stu-id="e5426-131">String</span></span>        | <span data-ttu-id="e5426-132">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="e5426-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="e5426-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="e5426-133">containerDisplayName</span></span>  | <span data-ttu-id="e5426-134">String</span><span class="sxs-lookup"><span data-stu-id="e5426-134">String</span></span>        | <span data-ttu-id="e5426-135">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="e5426-135">A string describing where the item is stored.</span></span> <span data-ttu-id="e5426-136">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="e5426-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="e5426-137">containerType</span><span class="sxs-lookup"><span data-stu-id="e5426-137">containerType</span></span>         | <span data-ttu-id="e5426-138">String</span><span class="sxs-lookup"><span data-stu-id="e5426-138">String</span></span> | <span data-ttu-id="e5426-139">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="e5426-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="e5426-140">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="e5426-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="e5426-141">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="e5426-141">Type property values</span></span>
-   <span data-ttu-id="e5426-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="e5426-142">PowerPoint</span></span>
-   <span data-ttu-id="e5426-143">Word</span><span class="sxs-lookup"><span data-stu-id="e5426-143">Word</span></span>
-   <span data-ttu-id="e5426-144">Excel</span><span class="sxs-lookup"><span data-stu-id="e5426-144">Excel</span></span>
-   <span data-ttu-id="e5426-145">Documento</span><span class="sxs-lookup"><span data-stu-id="e5426-145">Pdf</span></span>
-   <span data-ttu-id="e5426-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="e5426-146">OneNote</span></span>
-   <span data-ttu-id="e5426-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="e5426-147">OneNotePage</span></span>
-   <span data-ttu-id="e5426-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="e5426-148">InfoPath</span></span>
-   <span data-ttu-id="e5426-149">Visio</span><span class="sxs-lookup"><span data-stu-id="e5426-149">Visio</span></span>
-   <span data-ttu-id="e5426-150">Editor</span><span class="sxs-lookup"><span data-stu-id="e5426-150">Publisher</span></span>
-   <span data-ttu-id="e5426-151">Project</span><span class="sxs-lookup"><span data-stu-id="e5426-151">Project</span></span>
-   <span data-ttu-id="e5426-152">Access</span><span class="sxs-lookup"><span data-stu-id="e5426-152">Access</span></span>
-   <span data-ttu-id="e5426-153">Email</span><span class="sxs-lookup"><span data-stu-id="e5426-153">Mail</span></span>
-   <span data-ttu-id="e5426-154">Limit</span><span class="sxs-lookup"><span data-stu-id="e5426-154">Csv</span></span>
-   <span data-ttu-id="e5426-155">Arquivo</span><span class="sxs-lookup"><span data-stu-id="e5426-155">Archive</span></span>
-   <span data-ttu-id="e5426-156">XPS</span><span class="sxs-lookup"><span data-stu-id="e5426-156">Xps</span></span>
-   <span data-ttu-id="e5426-157">Áudio</span><span class="sxs-lookup"><span data-stu-id="e5426-157">Audio</span></span>
-   <span data-ttu-id="e5426-158">Vídeo</span><span class="sxs-lookup"><span data-stu-id="e5426-158">Video</span></span>
-   <span data-ttu-id="e5426-159">Image</span><span class="sxs-lookup"><span data-stu-id="e5426-159">Image</span></span>
-   <span data-ttu-id="e5426-160">Web</span><span class="sxs-lookup"><span data-stu-id="e5426-160">Web</span></span>
-   <span data-ttu-id="e5426-161">Texto</span><span class="sxs-lookup"><span data-stu-id="e5426-161">Text</span></span>
-   <span data-ttu-id="e5426-162">Xml</span><span class="sxs-lookup"><span data-stu-id="e5426-162">Xml</span></span>
-   <span data-ttu-id="e5426-163">História</span><span class="sxs-lookup"><span data-stu-id="e5426-163">Story</span></span>
-   <span data-ttu-id="e5426-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="e5426-164">ExternalContent</span></span>
-   <span data-ttu-id="e5426-165">Folder</span><span class="sxs-lookup"><span data-stu-id="e5426-165">Folder</span></span>
-   <span data-ttu-id="e5426-166">Other</span><span class="sxs-lookup"><span data-stu-id="e5426-166">Other</span></span>

<span data-ttu-id="e5426-167">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="e5426-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="e5426-168">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="e5426-168">containerType property values</span></span>
<span data-ttu-id="e5426-169">Os tipos com suporte podem diferir com base nos contêineres dos quais o [officeGraphInsights](officegraphinsights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="e5426-169">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="e5426-170">Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="e5426-170">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="e5426-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="e5426-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="e5426-172">Site</span><span class="sxs-lookup"><span data-stu-id="e5426-172">Site</span></span>
-   <span data-ttu-id="e5426-173">Email</span><span class="sxs-lookup"><span data-stu-id="e5426-173">Mail</span></span>
-   <span data-ttu-id="e5426-174">DropBox</span><span class="sxs-lookup"><span data-stu-id="e5426-174">DropBox</span></span>
-   <span data-ttu-id="e5426-175">Caixa</span><span class="sxs-lookup"><span data-stu-id="e5426-175">Box</span></span>
-   <span data-ttu-id="e5426-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="e5426-176">GDrive</span></span>

<span data-ttu-id="e5426-177">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="e5426-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
