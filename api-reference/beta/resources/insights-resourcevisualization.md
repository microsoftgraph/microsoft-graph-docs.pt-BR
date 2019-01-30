---
title: tipo de recurso de resourceVisualization
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641292"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="5c9e9-103">tipo de recurso de resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5c9e9-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c9e9-104">Tipo complexo que contém propriedades de [ideias](insights.md).</span><span class="sxs-lookup"><span data-stu-id="5c9e9-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c9e9-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c9e9-105">JSON representation</span></span>

<span data-ttu-id="5c9e9-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5c9e9-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="5c9e9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c9e9-107">Properties</span></span>

| <span data-ttu-id="5c9e9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c9e9-108">Property</span></span>              | <span data-ttu-id="5c9e9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c9e9-109">Type</span></span>          | <span data-ttu-id="5c9e9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c9e9-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="5c9e9-111">title</span><span class="sxs-lookup"><span data-stu-id="5c9e9-111">title</span></span>                 | <span data-ttu-id="5c9e9-112">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-112">String</span></span>        | <span data-ttu-id="5c9e9-113">Texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-113">The item's title text.</span></span>               |
| <span data-ttu-id="5c9e9-114">type</span><span class="sxs-lookup"><span data-stu-id="5c9e9-114">type</span></span>              | <span data-ttu-id="5c9e9-115">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-115">String</span></span>        | <span data-ttu-id="5c9e9-116">Tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-116">The item's media type.</span></span> <span data-ttu-id="5c9e9-117">Pode ser usado para filtrar para um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="5c9e9-118">Veja abaixo tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-118">See below for supported types.</span></span> |
| <span data-ttu-id="5c9e9-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="5c9e9-119">mediaType</span></span>             | <span data-ttu-id="5c9e9-120">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-120">String</span></span>        | <span data-ttu-id="5c9e9-121">Tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-121">The item's media type.</span></span> <span data-ttu-id="5c9e9-122">Pode ser usado para filtragem para um tipo específico de arquivo com base em tipos de Mime de mídia IANA suportados.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="5c9e9-123">Observe que nem todos os tipos de Mime de mídia são suportados.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="5c9e9-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="5c9e9-124">previewImageUrl</span></span>       | <span data-ttu-id="5c9e9-125">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-125">String</span></span>        | <span data-ttu-id="5c9e9-126">Uma URL, levando a imagem de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="5c9e9-127">previewText</span><span class="sxs-lookup"><span data-stu-id="5c9e9-127">previewText</span></span>           | <span data-ttu-id="5c9e9-128">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-128">String</span></span>        | <span data-ttu-id="5c9e9-129">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-129">A preview text for the item.</span></span> |
| <span data-ttu-id="5c9e9-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="5c9e9-130">containerWebUrl</span></span>       | <span data-ttu-id="5c9e9-131">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-131">String</span></span>        | <span data-ttu-id="5c9e9-132">Um caminho que leva à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="5c9e9-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="5c9e9-133">containerDisplayName</span></span>  | <span data-ttu-id="5c9e9-134">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-134">String</span></span>        | <span data-ttu-id="5c9e9-135">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-135">A string describing where the item is stored.</span></span> <span data-ttu-id="5c9e9-136">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive armazenar o item.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="5c9e9-137">containerType</span><span class="sxs-lookup"><span data-stu-id="5c9e9-137">containerType</span></span>         | <span data-ttu-id="5c9e9-138">String</span><span class="sxs-lookup"><span data-stu-id="5c9e9-138">String</span></span> | <span data-ttu-id="5c9e9-139">Pode ser usado para filtrar por tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="5c9e9-140">Como o Site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="5c9e9-141">Valores de tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="5c9e9-141">Type property values</span></span>
-   <span data-ttu-id="5c9e9-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="5c9e9-142">PowerPoint</span></span>
-   <span data-ttu-id="5c9e9-143">Word</span><span class="sxs-lookup"><span data-stu-id="5c9e9-143">Word</span></span>
-   <span data-ttu-id="5c9e9-144">Excel</span><span class="sxs-lookup"><span data-stu-id="5c9e9-144">Excel</span></span>
-   <span data-ttu-id="5c9e9-145">PDF</span><span class="sxs-lookup"><span data-stu-id="5c9e9-145">Pdf</span></span>
-   <span data-ttu-id="5c9e9-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="5c9e9-146">OneNote</span></span>
-   <span data-ttu-id="5c9e9-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="5c9e9-147">OneNotePage</span></span>
-   <span data-ttu-id="5c9e9-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="5c9e9-148">InfoPath</span></span>
-   <span data-ttu-id="5c9e9-149">Visio</span><span class="sxs-lookup"><span data-stu-id="5c9e9-149">Visio</span></span>
-   <span data-ttu-id="5c9e9-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="5c9e9-150">Publisher</span></span>
-   <span data-ttu-id="5c9e9-151">Project</span><span class="sxs-lookup"><span data-stu-id="5c9e9-151">Project</span></span>
-   <span data-ttu-id="5c9e9-152">Access</span><span class="sxs-lookup"><span data-stu-id="5c9e9-152">Access</span></span>
-   <span data-ttu-id="5c9e9-153">Email</span><span class="sxs-lookup"><span data-stu-id="5c9e9-153">Mail</span></span>
-   <span data-ttu-id="5c9e9-154">CSV</span><span class="sxs-lookup"><span data-stu-id="5c9e9-154">Csv</span></span>
-   <span data-ttu-id="5c9e9-155">Arquivo morto</span><span class="sxs-lookup"><span data-stu-id="5c9e9-155">Archive</span></span>
-   <span data-ttu-id="5c9e9-156">XPS</span><span class="sxs-lookup"><span data-stu-id="5c9e9-156">Xps</span></span>
-   <span data-ttu-id="5c9e9-157">Áudio</span><span class="sxs-lookup"><span data-stu-id="5c9e9-157">Audio</span></span>
-   <span data-ttu-id="5c9e9-158">Vídeo</span><span class="sxs-lookup"><span data-stu-id="5c9e9-158">Video</span></span>
-   <span data-ttu-id="5c9e9-159">Image</span><span class="sxs-lookup"><span data-stu-id="5c9e9-159">Image</span></span>
-   <span data-ttu-id="5c9e9-160">Web</span><span class="sxs-lookup"><span data-stu-id="5c9e9-160">Web</span></span>
-   <span data-ttu-id="5c9e9-161">Texto</span><span class="sxs-lookup"><span data-stu-id="5c9e9-161">Text</span></span>
-   <span data-ttu-id="5c9e9-162">Xml</span><span class="sxs-lookup"><span data-stu-id="5c9e9-162">Xml</span></span>
-   <span data-ttu-id="5c9e9-163">Story</span><span class="sxs-lookup"><span data-stu-id="5c9e9-163">Story</span></span>
-   <span data-ttu-id="5c9e9-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="5c9e9-164">ExternalContent</span></span>
-   <span data-ttu-id="5c9e9-165">Folder</span><span class="sxs-lookup"><span data-stu-id="5c9e9-165">Folder</span></span>
-   <span data-ttu-id="5c9e9-166">Other</span><span class="sxs-lookup"><span data-stu-id="5c9e9-166">Other</span></span>

<span data-ttu-id="5c9e9-167">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="5c9e9-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="5c9e9-168">valores de propriedade containerType</span><span class="sxs-lookup"><span data-stu-id="5c9e9-168">containerType property values</span></span>
<span data-ttu-id="5c9e9-169">Os tipos suportados podem variar, dependendo em contêineres do qual a [percepção](insights.md) retorna os arquivos.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="5c9e9-170">Por exemplo, apenas o insight [compartilhados](insights-shared.md) retorna arquivos do 'Recados', 'Caixa' e 'GDrive'.</span><span class="sxs-lookup"><span data-stu-id="5c9e9-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="5c9e9-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="5c9e9-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="5c9e9-172">Site</span><span class="sxs-lookup"><span data-stu-id="5c9e9-172">Site</span></span>
-   <span data-ttu-id="5c9e9-173">Email</span><span class="sxs-lookup"><span data-stu-id="5c9e9-173">Mail</span></span>
-   <span data-ttu-id="5c9e9-174">Pasta de recados</span><span class="sxs-lookup"><span data-stu-id="5c9e9-174">DropBox</span></span>
-   <span data-ttu-id="5c9e9-175">Caixa</span><span class="sxs-lookup"><span data-stu-id="5c9e9-175">Box</span></span>
-   <span data-ttu-id="5c9e9-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="5c9e9-176">GDrive</span></span>

<span data-ttu-id="5c9e9-177">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="5c9e9-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
