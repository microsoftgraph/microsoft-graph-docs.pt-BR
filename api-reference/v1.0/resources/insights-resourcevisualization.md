---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2480f55cf0e7ea12d9bfaf31941a943095f62c31
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898034"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="81abb-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="81abb-103">resourceVisualization resource type</span></span>

<span data-ttu-id="81abb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81abb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81abb-105">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="81abb-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="81abb-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81abb-106">JSON representation</span></span>

<span data-ttu-id="81abb-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="81abb-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="81abb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81abb-108">Properties</span></span>

| <span data-ttu-id="81abb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81abb-109">Property</span></span>              | <span data-ttu-id="81abb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="81abb-110">Type</span></span>          | <span data-ttu-id="81abb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="81abb-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="81abb-112">title</span><span class="sxs-lookup"><span data-stu-id="81abb-112">title</span></span>                 | <span data-ttu-id="81abb-113">String</span><span class="sxs-lookup"><span data-stu-id="81abb-113">String</span></span>        | <span data-ttu-id="81abb-114">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="81abb-114">The item's title text.</span></span>               |
| <span data-ttu-id="81abb-115">tipo</span><span class="sxs-lookup"><span data-stu-id="81abb-115">type</span></span>              | <span data-ttu-id="81abb-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81abb-116">String</span></span>        | <span data-ttu-id="81abb-117">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="81abb-117">The item's media type.</span></span> <span data-ttu-id="81abb-118">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="81abb-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="81abb-119">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="81abb-119">See below for supported types.</span></span> |
| <span data-ttu-id="81abb-120">Mídia</span><span class="sxs-lookup"><span data-stu-id="81abb-120">mediaType</span></span>             | <span data-ttu-id="81abb-121">String</span><span class="sxs-lookup"><span data-stu-id="81abb-121">String</span></span>        | <span data-ttu-id="81abb-122">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="81abb-122">The item's media type.</span></span> <span data-ttu-id="81abb-123">Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="81abb-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="81abb-124">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="81abb-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="81abb-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="81abb-125">previewImageUrl</span></span>       | <span data-ttu-id="81abb-126">String</span><span class="sxs-lookup"><span data-stu-id="81abb-126">String</span></span>        | <span data-ttu-id="81abb-127">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="81abb-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="81abb-128">previewText</span><span class="sxs-lookup"><span data-stu-id="81abb-128">previewText</span></span>           | <span data-ttu-id="81abb-129">String</span><span class="sxs-lookup"><span data-stu-id="81abb-129">String</span></span>        | <span data-ttu-id="81abb-130">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="81abb-130">A preview text for the item.</span></span> |
| <span data-ttu-id="81abb-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="81abb-131">containerWebUrl</span></span>       | <span data-ttu-id="81abb-132">String</span><span class="sxs-lookup"><span data-stu-id="81abb-132">String</span></span>        | <span data-ttu-id="81abb-133">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="81abb-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="81abb-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="81abb-134">containerDisplayName</span></span>  | <span data-ttu-id="81abb-135">String</span><span class="sxs-lookup"><span data-stu-id="81abb-135">String</span></span>        | <span data-ttu-id="81abb-136">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="81abb-136">A string describing where the item is stored.</span></span> <span data-ttu-id="81abb-137">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="81abb-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="81abb-138">containerType</span><span class="sxs-lookup"><span data-stu-id="81abb-138">containerType</span></span>         | <span data-ttu-id="81abb-139">String</span><span class="sxs-lookup"><span data-stu-id="81abb-139">String</span></span> | <span data-ttu-id="81abb-140">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="81abb-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="81abb-141">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="81abb-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="81abb-142">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="81abb-142">Type property values</span></span>
-   <span data-ttu-id="81abb-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="81abb-143">PowerPoint</span></span>
-   <span data-ttu-id="81abb-144">Word</span><span class="sxs-lookup"><span data-stu-id="81abb-144">Word</span></span>
-   <span data-ttu-id="81abb-145">Excel</span><span class="sxs-lookup"><span data-stu-id="81abb-145">Excel</span></span>
-   <span data-ttu-id="81abb-146">Documento</span><span class="sxs-lookup"><span data-stu-id="81abb-146">Pdf</span></span>
-   <span data-ttu-id="81abb-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="81abb-147">OneNote</span></span>
-   <span data-ttu-id="81abb-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="81abb-148">OneNotePage</span></span>
-   <span data-ttu-id="81abb-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="81abb-149">InfoPath</span></span>
-   <span data-ttu-id="81abb-150">Visio</span><span class="sxs-lookup"><span data-stu-id="81abb-150">Visio</span></span>
-   <span data-ttu-id="81abb-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="81abb-151">Publisher</span></span>
-   <span data-ttu-id="81abb-152">Project</span><span class="sxs-lookup"><span data-stu-id="81abb-152">Project</span></span>
-   <span data-ttu-id="81abb-153">Access</span><span class="sxs-lookup"><span data-stu-id="81abb-153">Access</span></span>
-   <span data-ttu-id="81abb-154">Correio</span><span class="sxs-lookup"><span data-stu-id="81abb-154">Mail</span></span>
-   <span data-ttu-id="81abb-155">Limit</span><span class="sxs-lookup"><span data-stu-id="81abb-155">Csv</span></span>
-   <span data-ttu-id="81abb-156">Arquivar</span><span class="sxs-lookup"><span data-stu-id="81abb-156">Archive</span></span>
-   <span data-ttu-id="81abb-157">XPS</span><span class="sxs-lookup"><span data-stu-id="81abb-157">Xps</span></span>
-   <span data-ttu-id="81abb-158">Áudio</span><span class="sxs-lookup"><span data-stu-id="81abb-158">Audio</span></span>
-   <span data-ttu-id="81abb-159">Vídeo</span><span class="sxs-lookup"><span data-stu-id="81abb-159">Video</span></span>
-   <span data-ttu-id="81abb-160">Image</span><span class="sxs-lookup"><span data-stu-id="81abb-160">Image</span></span>
-   <span data-ttu-id="81abb-161">Web</span><span class="sxs-lookup"><span data-stu-id="81abb-161">Web</span></span>
-   <span data-ttu-id="81abb-162">Texto</span><span class="sxs-lookup"><span data-stu-id="81abb-162">Text</span></span>
-   <span data-ttu-id="81abb-163">Xml</span><span class="sxs-lookup"><span data-stu-id="81abb-163">Xml</span></span>
-   <span data-ttu-id="81abb-164">História</span><span class="sxs-lookup"><span data-stu-id="81abb-164">Story</span></span>
-   <span data-ttu-id="81abb-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="81abb-165">ExternalContent</span></span>
-   <span data-ttu-id="81abb-166">Folder</span><span class="sxs-lookup"><span data-stu-id="81abb-166">Folder</span></span>
- <span data-ttu-id="81abb-167">SPSite</span><span class="sxs-lookup"><span data-stu-id="81abb-167">Spsite</span></span>
-   <span data-ttu-id="81abb-168">Outros</span><span class="sxs-lookup"><span data-stu-id="81abb-168">Other</span></span>

<span data-ttu-id="81abb-169">Consulta de exemplo:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="81abb-169">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

<span data-ttu-id="81abb-170">Observações: `spsite` talvez seja necessário classificar por `lastUsed/lastAccessedDateTime` desc para recuperar resultados válidos</span><span class="sxs-lookup"><span data-stu-id="81abb-170">Notes: For `spsite` you may need to sort by `lastUsed/lastAccessedDateTime` desc in order to retrieve valid results</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="81abb-171">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="81abb-171">containerType property values</span></span>
<span data-ttu-id="81abb-172">Os tipos com suporte podem diferir com base nos contêineres dos quais o [officeGraphInsights](officegraphinsights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="81abb-172">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="81abb-173">Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="81abb-173">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="81abb-174">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="81abb-174">OneDriveBusiness</span></span>
-   <span data-ttu-id="81abb-175">Site</span><span class="sxs-lookup"><span data-stu-id="81abb-175">Site</span></span>
-   <span data-ttu-id="81abb-176">Correio</span><span class="sxs-lookup"><span data-stu-id="81abb-176">Mail</span></span>
-   <span data-ttu-id="81abb-177">DropBox</span><span class="sxs-lookup"><span data-stu-id="81abb-177">DropBox</span></span>
-   <span data-ttu-id="81abb-178">Caixa</span><span class="sxs-lookup"><span data-stu-id="81abb-178">Box</span></span>
-   <span data-ttu-id="81abb-179">GDrive</span><span class="sxs-lookup"><span data-stu-id="81abb-179">GDrive</span></span>

<span data-ttu-id="81abb-180">Consulta de exemplo:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="81abb-180">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
