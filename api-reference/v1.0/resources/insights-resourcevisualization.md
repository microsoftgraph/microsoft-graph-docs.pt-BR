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
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="3d7cd-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="3d7cd-103">resourceVisualization resource type</span></span>

<span data-ttu-id="3d7cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d7cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d7cd-105">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="3d7cd-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d7cd-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d7cd-106">JSON representation</span></span>

<span data-ttu-id="3d7cd-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3d7cd-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3d7cd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d7cd-108">Properties</span></span>

| <span data-ttu-id="3d7cd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d7cd-109">Property</span></span>              | <span data-ttu-id="3d7cd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d7cd-110">Type</span></span>          | <span data-ttu-id="3d7cd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d7cd-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="3d7cd-112">title</span><span class="sxs-lookup"><span data-stu-id="3d7cd-112">title</span></span>                 | <span data-ttu-id="3d7cd-113">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-113">String</span></span>        | <span data-ttu-id="3d7cd-114">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-114">The item's title text.</span></span>               |
| <span data-ttu-id="3d7cd-115">tipo</span><span class="sxs-lookup"><span data-stu-id="3d7cd-115">type</span></span>              | <span data-ttu-id="3d7cd-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7cd-116">String</span></span>        | <span data-ttu-id="3d7cd-117">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-117">The item's media type.</span></span> <span data-ttu-id="3d7cd-118">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="3d7cd-119">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-119">See below for supported types.</span></span> |
| <span data-ttu-id="3d7cd-120">Mídia</span><span class="sxs-lookup"><span data-stu-id="3d7cd-120">mediaType</span></span>             | <span data-ttu-id="3d7cd-121">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-121">String</span></span>        | <span data-ttu-id="3d7cd-122">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-122">The item's media type.</span></span> <span data-ttu-id="3d7cd-123">Pode ser usado para filtragem de um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="3d7cd-124">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="3d7cd-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="3d7cd-125">previewImageUrl</span></span>       | <span data-ttu-id="3d7cd-126">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-126">String</span></span>        | <span data-ttu-id="3d7cd-127">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="3d7cd-128">previewText</span><span class="sxs-lookup"><span data-stu-id="3d7cd-128">previewText</span></span>           | <span data-ttu-id="3d7cd-129">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-129">String</span></span>        | <span data-ttu-id="3d7cd-130">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-130">A preview text for the item.</span></span> |
| <span data-ttu-id="3d7cd-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="3d7cd-131">containerWebUrl</span></span>       | <span data-ttu-id="3d7cd-132">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-132">String</span></span>        | <span data-ttu-id="3d7cd-133">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="3d7cd-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d7cd-134">containerDisplayName</span></span>  | <span data-ttu-id="3d7cd-135">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-135">String</span></span>        | <span data-ttu-id="3d7cd-136">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-136">A string describing where the item is stored.</span></span> <span data-ttu-id="3d7cd-137">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="3d7cd-138">containerType</span><span class="sxs-lookup"><span data-stu-id="3d7cd-138">containerType</span></span>         | <span data-ttu-id="3d7cd-139">String</span><span class="sxs-lookup"><span data-stu-id="3d7cd-139">String</span></span> | <span data-ttu-id="3d7cd-140">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="3d7cd-141">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="3d7cd-142">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="3d7cd-142">Type property values</span></span>
-   <span data-ttu-id="3d7cd-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="3d7cd-143">PowerPoint</span></span>
-   <span data-ttu-id="3d7cd-144">Word</span><span class="sxs-lookup"><span data-stu-id="3d7cd-144">Word</span></span>
-   <span data-ttu-id="3d7cd-145">Excel</span><span class="sxs-lookup"><span data-stu-id="3d7cd-145">Excel</span></span>
-   <span data-ttu-id="3d7cd-146">Documento</span><span class="sxs-lookup"><span data-stu-id="3d7cd-146">Pdf</span></span>
-   <span data-ttu-id="3d7cd-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="3d7cd-147">OneNote</span></span>
-   <span data-ttu-id="3d7cd-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="3d7cd-148">OneNotePage</span></span>
-   <span data-ttu-id="3d7cd-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="3d7cd-149">InfoPath</span></span>
-   <span data-ttu-id="3d7cd-150">Visio</span><span class="sxs-lookup"><span data-stu-id="3d7cd-150">Visio</span></span>
-   <span data-ttu-id="3d7cd-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="3d7cd-151">Publisher</span></span>
-   <span data-ttu-id="3d7cd-152">Project</span><span class="sxs-lookup"><span data-stu-id="3d7cd-152">Project</span></span>
-   <span data-ttu-id="3d7cd-153">Access</span><span class="sxs-lookup"><span data-stu-id="3d7cd-153">Access</span></span>
-   <span data-ttu-id="3d7cd-154">Correio</span><span class="sxs-lookup"><span data-stu-id="3d7cd-154">Mail</span></span>
-   <span data-ttu-id="3d7cd-155">Limit</span><span class="sxs-lookup"><span data-stu-id="3d7cd-155">Csv</span></span>
-   <span data-ttu-id="3d7cd-156">Arquivar</span><span class="sxs-lookup"><span data-stu-id="3d7cd-156">Archive</span></span>
-   <span data-ttu-id="3d7cd-157">XPS</span><span class="sxs-lookup"><span data-stu-id="3d7cd-157">Xps</span></span>
-   <span data-ttu-id="3d7cd-158">Áudio</span><span class="sxs-lookup"><span data-stu-id="3d7cd-158">Audio</span></span>
-   <span data-ttu-id="3d7cd-159">Vídeo</span><span class="sxs-lookup"><span data-stu-id="3d7cd-159">Video</span></span>
-   <span data-ttu-id="3d7cd-160">Image</span><span class="sxs-lookup"><span data-stu-id="3d7cd-160">Image</span></span>
-   <span data-ttu-id="3d7cd-161">Web</span><span class="sxs-lookup"><span data-stu-id="3d7cd-161">Web</span></span>
-   <span data-ttu-id="3d7cd-162">Texto</span><span class="sxs-lookup"><span data-stu-id="3d7cd-162">Text</span></span>
-   <span data-ttu-id="3d7cd-163">Xml</span><span class="sxs-lookup"><span data-stu-id="3d7cd-163">Xml</span></span>
-   <span data-ttu-id="3d7cd-164">História</span><span class="sxs-lookup"><span data-stu-id="3d7cd-164">Story</span></span>
-   <span data-ttu-id="3d7cd-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="3d7cd-165">ExternalContent</span></span>
-   <span data-ttu-id="3d7cd-166">Folder</span><span class="sxs-lookup"><span data-stu-id="3d7cd-166">Folder</span></span>
- <span data-ttu-id="3d7cd-167">SPSite</span><span class="sxs-lookup"><span data-stu-id="3d7cd-167">Spsite</span></span>
-   <span data-ttu-id="3d7cd-168">Outros</span><span class="sxs-lookup"><span data-stu-id="3d7cd-168">Other</span></span>

<span data-ttu-id="3d7cd-169">Consulta de exemplo:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="3d7cd-169">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

<span data-ttu-id="3d7cd-170">Observações: `spsite` talvez seja necessário classificar por `lastUsed/lastAccessedDateTime` desc para recuperar resultados válidos</span><span class="sxs-lookup"><span data-stu-id="3d7cd-170">Notes: For `spsite` you may need to sort by `lastUsed/lastAccessedDateTime` desc in order to retrieve valid results</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="3d7cd-171">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="3d7cd-171">containerType property values</span></span>
<span data-ttu-id="3d7cd-172">Os tipos com suporte podem diferir com base nos contêineres dos quais o [officeGraphInsights](officegraphinsights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="3d7cd-172">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="3d7cd-173">Por exemplo, somente a percepção [sharedInsight](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="3d7cd-173">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="3d7cd-174">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="3d7cd-174">OneDriveBusiness</span></span>
-   <span data-ttu-id="3d7cd-175">Site</span><span class="sxs-lookup"><span data-stu-id="3d7cd-175">Site</span></span>
-   <span data-ttu-id="3d7cd-176">Correio</span><span class="sxs-lookup"><span data-stu-id="3d7cd-176">Mail</span></span>
-   <span data-ttu-id="3d7cd-177">DropBox</span><span class="sxs-lookup"><span data-stu-id="3d7cd-177">DropBox</span></span>
-   <span data-ttu-id="3d7cd-178">Caixa</span><span class="sxs-lookup"><span data-stu-id="3d7cd-178">Box</span></span>
-   <span data-ttu-id="3d7cd-179">GDrive</span><span class="sxs-lookup"><span data-stu-id="3d7cd-179">GDrive</span></span>

<span data-ttu-id="3d7cd-180">Consulta de exemplo:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="3d7cd-180">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
