---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 93adb5c8dcef2cb7472d2f58385f8c2a779566c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054816"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="921ed-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="921ed-103">resourceVisualization resource type</span></span>

<span data-ttu-id="921ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="921ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="921ed-105">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="921ed-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="921ed-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="921ed-106">JSON representation</span></span>

<span data-ttu-id="921ed-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="921ed-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="921ed-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="921ed-108">Properties</span></span>

| <span data-ttu-id="921ed-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="921ed-109">Property</span></span>              | <span data-ttu-id="921ed-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="921ed-110">Type</span></span>          | <span data-ttu-id="921ed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="921ed-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="921ed-112">title</span><span class="sxs-lookup"><span data-stu-id="921ed-112">title</span></span>                 | <span data-ttu-id="921ed-113">String</span><span class="sxs-lookup"><span data-stu-id="921ed-113">String</span></span>        | <span data-ttu-id="921ed-114">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="921ed-114">The item's title text.</span></span>               |
| <span data-ttu-id="921ed-115">tipo</span><span class="sxs-lookup"><span data-stu-id="921ed-115">type</span></span>              | <span data-ttu-id="921ed-116">String</span><span class="sxs-lookup"><span data-stu-id="921ed-116">String</span></span>        | <span data-ttu-id="921ed-117">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="921ed-117">The item's media type.</span></span> <span data-ttu-id="921ed-118">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="921ed-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="921ed-119">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="921ed-119">See below for supported types.</span></span> |
| <span data-ttu-id="921ed-120">mediaType</span><span class="sxs-lookup"><span data-stu-id="921ed-120">mediaType</span></span>             | <span data-ttu-id="921ed-121">String</span><span class="sxs-lookup"><span data-stu-id="921ed-121">String</span></span>        | <span data-ttu-id="921ed-122">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="921ed-122">The item's media type.</span></span> <span data-ttu-id="921ed-123">Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="921ed-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="921ed-124">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="921ed-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="921ed-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="921ed-125">previewImageUrl</span></span>       | <span data-ttu-id="921ed-126">String</span><span class="sxs-lookup"><span data-stu-id="921ed-126">String</span></span>        | <span data-ttu-id="921ed-127">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="921ed-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="921ed-128">previewText</span><span class="sxs-lookup"><span data-stu-id="921ed-128">previewText</span></span>           | <span data-ttu-id="921ed-129">String</span><span class="sxs-lookup"><span data-stu-id="921ed-129">String</span></span>        | <span data-ttu-id="921ed-130">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="921ed-130">A preview text for the item.</span></span> |
| <span data-ttu-id="921ed-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="921ed-131">containerWebUrl</span></span>       | <span data-ttu-id="921ed-132">String</span><span class="sxs-lookup"><span data-stu-id="921ed-132">String</span></span>        | <span data-ttu-id="921ed-133">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="921ed-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="921ed-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="921ed-134">containerDisplayName</span></span>  | <span data-ttu-id="921ed-135">String</span><span class="sxs-lookup"><span data-stu-id="921ed-135">String</span></span>        | <span data-ttu-id="921ed-136">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="921ed-136">A string describing where the item is stored.</span></span> <span data-ttu-id="921ed-137">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="921ed-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="921ed-138">containerType</span><span class="sxs-lookup"><span data-stu-id="921ed-138">containerType</span></span>         | <span data-ttu-id="921ed-139">String</span><span class="sxs-lookup"><span data-stu-id="921ed-139">String</span></span> | <span data-ttu-id="921ed-140">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="921ed-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="921ed-141">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="921ed-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="921ed-142">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="921ed-142">Type property values</span></span>
-   <span data-ttu-id="921ed-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="921ed-143">PowerPoint</span></span>
-   <span data-ttu-id="921ed-144">Word</span><span class="sxs-lookup"><span data-stu-id="921ed-144">Word</span></span>
-   <span data-ttu-id="921ed-145">Excel</span><span class="sxs-lookup"><span data-stu-id="921ed-145">Excel</span></span>
-   <span data-ttu-id="921ed-146">Documento</span><span class="sxs-lookup"><span data-stu-id="921ed-146">Pdf</span></span>
-   <span data-ttu-id="921ed-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="921ed-147">OneNote</span></span>
-   <span data-ttu-id="921ed-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="921ed-148">OneNotePage</span></span>
-   <span data-ttu-id="921ed-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="921ed-149">InfoPath</span></span>
-   <span data-ttu-id="921ed-150">Visio</span><span class="sxs-lookup"><span data-stu-id="921ed-150">Visio</span></span>
-   <span data-ttu-id="921ed-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="921ed-151">Publisher</span></span>
-   <span data-ttu-id="921ed-152">Project</span><span class="sxs-lookup"><span data-stu-id="921ed-152">Project</span></span>
-   <span data-ttu-id="921ed-153">Access</span><span class="sxs-lookup"><span data-stu-id="921ed-153">Access</span></span>
-   <span data-ttu-id="921ed-154">Email</span><span class="sxs-lookup"><span data-stu-id="921ed-154">Mail</span></span>
-   <span data-ttu-id="921ed-155">Limit</span><span class="sxs-lookup"><span data-stu-id="921ed-155">Csv</span></span>
-   <span data-ttu-id="921ed-156">Arquivar</span><span class="sxs-lookup"><span data-stu-id="921ed-156">Archive</span></span>
-   <span data-ttu-id="921ed-157">XPS</span><span class="sxs-lookup"><span data-stu-id="921ed-157">Xps</span></span>
-   <span data-ttu-id="921ed-158">Áudio</span><span class="sxs-lookup"><span data-stu-id="921ed-158">Audio</span></span>
-   <span data-ttu-id="921ed-159">Vídeo</span><span class="sxs-lookup"><span data-stu-id="921ed-159">Video</span></span>
-   <span data-ttu-id="921ed-160">Imagem</span><span class="sxs-lookup"><span data-stu-id="921ed-160">Image</span></span>
-   <span data-ttu-id="921ed-161">Web</span><span class="sxs-lookup"><span data-stu-id="921ed-161">Web</span></span>
-   <span data-ttu-id="921ed-162">Texto</span><span class="sxs-lookup"><span data-stu-id="921ed-162">Text</span></span>
-   <span data-ttu-id="921ed-163">Xml</span><span class="sxs-lookup"><span data-stu-id="921ed-163">Xml</span></span>
-   <span data-ttu-id="921ed-164">História</span><span class="sxs-lookup"><span data-stu-id="921ed-164">Story</span></span>
-   <span data-ttu-id="921ed-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="921ed-165">ExternalContent</span></span>
-   <span data-ttu-id="921ed-166">Folder</span><span class="sxs-lookup"><span data-stu-id="921ed-166">Folder</span></span>
- <span data-ttu-id="921ed-167">SPSite</span><span class="sxs-lookup"><span data-stu-id="921ed-167">Spsite</span></span>
-   <span data-ttu-id="921ed-168">Outros</span><span class="sxs-lookup"><span data-stu-id="921ed-168">Other</span></span>

<span data-ttu-id="921ed-169">Consulta de exemplo: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="921ed-169">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

<span data-ttu-id="921ed-170">Observações: `spsite` talvez seja necessário classificar por `lastUsed/lastAccessedDateTime` desc para recuperar resultados válidos</span><span class="sxs-lookup"><span data-stu-id="921ed-170">Notes: For `spsite` you may need to sort by `lastUsed/lastAccessedDateTime` desc in order to retrieve valid results</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="921ed-171">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="921ed-171">containerType property values</span></span>
<span data-ttu-id="921ed-172">Os tipos com suporte podem diferir com base nos contêineres dos quais o [officeGraphInsights](officegraphinsights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="921ed-172">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="921ed-173">Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="921ed-173">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="921ed-174">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="921ed-174">OneDriveBusiness</span></span>
-   <span data-ttu-id="921ed-175">Site</span><span class="sxs-lookup"><span data-stu-id="921ed-175">Site</span></span>
-   <span data-ttu-id="921ed-176">Email</span><span class="sxs-lookup"><span data-stu-id="921ed-176">Mail</span></span>
-   <span data-ttu-id="921ed-177">DropBox</span><span class="sxs-lookup"><span data-stu-id="921ed-177">DropBox</span></span>
-   <span data-ttu-id="921ed-178">Caixa</span><span class="sxs-lookup"><span data-stu-id="921ed-178">Box</span></span>
-   <span data-ttu-id="921ed-179">GDrive</span><span class="sxs-lookup"><span data-stu-id="921ed-179">GDrive</span></span>

<span data-ttu-id="921ed-180">Consulta de exemplo: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="921ed-180">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>

