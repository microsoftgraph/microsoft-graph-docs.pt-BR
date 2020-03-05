---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cb782ff0090c5e89e4a87f86af75f3fb51bb8251
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495652"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="10121-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="10121-103">resourceVisualization resource type</span></span>

<span data-ttu-id="10121-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="10121-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10121-105">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="10121-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="10121-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10121-106">JSON representation</span></span>

<span data-ttu-id="10121-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="10121-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="10121-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10121-108">Properties</span></span>

| <span data-ttu-id="10121-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10121-109">Property</span></span>              | <span data-ttu-id="10121-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="10121-110">Type</span></span>          | <span data-ttu-id="10121-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="10121-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="10121-112">title</span><span class="sxs-lookup"><span data-stu-id="10121-112">title</span></span>                 | <span data-ttu-id="10121-113">String</span><span class="sxs-lookup"><span data-stu-id="10121-113">String</span></span>        | <span data-ttu-id="10121-114">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="10121-114">The item's title text.</span></span>               |
| <span data-ttu-id="10121-115">type</span><span class="sxs-lookup"><span data-stu-id="10121-115">type</span></span>              | <span data-ttu-id="10121-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10121-116">String</span></span>        | <span data-ttu-id="10121-117">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="10121-117">The item's media type.</span></span> <span data-ttu-id="10121-118">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="10121-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="10121-119">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="10121-119">See below for supported types.</span></span> |
| <span data-ttu-id="10121-120">Mídia</span><span class="sxs-lookup"><span data-stu-id="10121-120">mediaType</span></span>             | <span data-ttu-id="10121-121">String</span><span class="sxs-lookup"><span data-stu-id="10121-121">String</span></span>        | <span data-ttu-id="10121-122">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="10121-122">The item's media type.</span></span> <span data-ttu-id="10121-123">Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="10121-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="10121-124">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="10121-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="10121-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="10121-125">previewImageUrl</span></span>       | <span data-ttu-id="10121-126">String</span><span class="sxs-lookup"><span data-stu-id="10121-126">String</span></span>        | <span data-ttu-id="10121-127">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="10121-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="10121-128">previewText</span><span class="sxs-lookup"><span data-stu-id="10121-128">previewText</span></span>           | <span data-ttu-id="10121-129">String</span><span class="sxs-lookup"><span data-stu-id="10121-129">String</span></span>        | <span data-ttu-id="10121-130">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="10121-130">A preview text for the item.</span></span> |
| <span data-ttu-id="10121-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="10121-131">containerWebUrl</span></span>       | <span data-ttu-id="10121-132">String</span><span class="sxs-lookup"><span data-stu-id="10121-132">String</span></span>        | <span data-ttu-id="10121-133">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="10121-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="10121-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="10121-134">containerDisplayName</span></span>  | <span data-ttu-id="10121-135">String</span><span class="sxs-lookup"><span data-stu-id="10121-135">String</span></span>        | <span data-ttu-id="10121-136">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="10121-136">A string describing where the item is stored.</span></span> <span data-ttu-id="10121-137">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="10121-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="10121-138">containerType</span><span class="sxs-lookup"><span data-stu-id="10121-138">containerType</span></span>         | <span data-ttu-id="10121-139">String</span><span class="sxs-lookup"><span data-stu-id="10121-139">String</span></span> | <span data-ttu-id="10121-140">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="10121-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="10121-141">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="10121-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="10121-142">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="10121-142">Type property values</span></span>
-   <span data-ttu-id="10121-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="10121-143">PowerPoint</span></span>
-   <span data-ttu-id="10121-144">Word</span><span class="sxs-lookup"><span data-stu-id="10121-144">Word</span></span>
-   <span data-ttu-id="10121-145">Excel</span><span class="sxs-lookup"><span data-stu-id="10121-145">Excel</span></span>
-   <span data-ttu-id="10121-146">Documento</span><span class="sxs-lookup"><span data-stu-id="10121-146">Pdf</span></span>
-   <span data-ttu-id="10121-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="10121-147">OneNote</span></span>
-   <span data-ttu-id="10121-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="10121-148">OneNotePage</span></span>
-   <span data-ttu-id="10121-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="10121-149">InfoPath</span></span>
-   <span data-ttu-id="10121-150">Visio</span><span class="sxs-lookup"><span data-stu-id="10121-150">Visio</span></span>
-   <span data-ttu-id="10121-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="10121-151">Publisher</span></span>
-   <span data-ttu-id="10121-152">Project</span><span class="sxs-lookup"><span data-stu-id="10121-152">Project</span></span>
-   <span data-ttu-id="10121-153">Access</span><span class="sxs-lookup"><span data-stu-id="10121-153">Access</span></span>
-   <span data-ttu-id="10121-154">Email</span><span class="sxs-lookup"><span data-stu-id="10121-154">Mail</span></span>
-   <span data-ttu-id="10121-155">Limit</span><span class="sxs-lookup"><span data-stu-id="10121-155">Csv</span></span>
-   <span data-ttu-id="10121-156">Arquivo</span><span class="sxs-lookup"><span data-stu-id="10121-156">Archive</span></span>
-   <span data-ttu-id="10121-157">XPS</span><span class="sxs-lookup"><span data-stu-id="10121-157">Xps</span></span>
-   <span data-ttu-id="10121-158">Áudio</span><span class="sxs-lookup"><span data-stu-id="10121-158">Audio</span></span>
-   <span data-ttu-id="10121-159">Vídeo</span><span class="sxs-lookup"><span data-stu-id="10121-159">Video</span></span>
-   <span data-ttu-id="10121-160">Image</span><span class="sxs-lookup"><span data-stu-id="10121-160">Image</span></span>
-   <span data-ttu-id="10121-161">Web</span><span class="sxs-lookup"><span data-stu-id="10121-161">Web</span></span>
-   <span data-ttu-id="10121-162">Texto</span><span class="sxs-lookup"><span data-stu-id="10121-162">Text</span></span>
-   <span data-ttu-id="10121-163">Xml</span><span class="sxs-lookup"><span data-stu-id="10121-163">Xml</span></span>
-   <span data-ttu-id="10121-164">História</span><span class="sxs-lookup"><span data-stu-id="10121-164">Story</span></span>
-   <span data-ttu-id="10121-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="10121-165">ExternalContent</span></span>
-   <span data-ttu-id="10121-166">Folder</span><span class="sxs-lookup"><span data-stu-id="10121-166">Folder</span></span>
-   <span data-ttu-id="10121-167">Outros</span><span class="sxs-lookup"><span data-stu-id="10121-167">Other</span></span>

<span data-ttu-id="10121-168">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="10121-168">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="10121-169">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="10121-169">containerType property values</span></span>
<span data-ttu-id="10121-170">Os tipos com suporte podem diferir com base nos contêineres dos quais o [officeGraphInsights](officegraphinsights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="10121-170">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="10121-171">Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="10121-171">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="10121-172">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="10121-172">OneDriveBusiness</span></span>
-   <span data-ttu-id="10121-173">Site</span><span class="sxs-lookup"><span data-stu-id="10121-173">Site</span></span>
-   <span data-ttu-id="10121-174">Email</span><span class="sxs-lookup"><span data-stu-id="10121-174">Mail</span></span>
-   <span data-ttu-id="10121-175">DropBox</span><span class="sxs-lookup"><span data-stu-id="10121-175">DropBox</span></span>
-   <span data-ttu-id="10121-176">Caixa</span><span class="sxs-lookup"><span data-stu-id="10121-176">Box</span></span>
-   <span data-ttu-id="10121-177">GDrive</span><span class="sxs-lookup"><span data-stu-id="10121-177">GDrive</span></span>

<span data-ttu-id="10121-178">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="10121-178">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
