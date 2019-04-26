---
title: tipo de recurso resourceVisualization
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550732"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="71dfc-103">tipo de recurso resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="71dfc-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71dfc-104">Tipo complexo contendo propriedades de [](insights.md)insights.</span><span class="sxs-lookup"><span data-stu-id="71dfc-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="71dfc-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71dfc-105">JSON representation</span></span>

<span data-ttu-id="71dfc-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="71dfc-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="71dfc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71dfc-107">Properties</span></span>

| <span data-ttu-id="71dfc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71dfc-108">Property</span></span>              | <span data-ttu-id="71dfc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="71dfc-109">Type</span></span>          | <span data-ttu-id="71dfc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71dfc-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="71dfc-111">title</span><span class="sxs-lookup"><span data-stu-id="71dfc-111">title</span></span>                 | <span data-ttu-id="71dfc-112">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-112">String</span></span>        | <span data-ttu-id="71dfc-113">O texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="71dfc-113">The item's title text.</span></span>               |
| <span data-ttu-id="71dfc-114">type</span><span class="sxs-lookup"><span data-stu-id="71dfc-114">type</span></span>              | <span data-ttu-id="71dfc-115">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-115">String</span></span>        | <span data-ttu-id="71dfc-116">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="71dfc-116">The item's media type.</span></span> <span data-ttu-id="71dfc-117">Pode ser usado para filtrar um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="71dfc-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="71dfc-118">Veja abaixo os tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="71dfc-118">See below for supported types.</span></span> |
| <span data-ttu-id="71dfc-119">Mídia</span><span class="sxs-lookup"><span data-stu-id="71dfc-119">mediaType</span></span>             | <span data-ttu-id="71dfc-120">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-120">String</span></span>        | <span data-ttu-id="71dfc-121">O tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="71dfc-121">The item's media type.</span></span> <span data-ttu-id="71dfc-122">Pode ser usado para filtragem para um tipo específico de arquivo baseado em tipos MIME de mídias da IANA compatíveis.</span><span class="sxs-lookup"><span data-stu-id="71dfc-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="71dfc-123">Observe que nem todos os tipos de MIME de mídia têm suporte.</span><span class="sxs-lookup"><span data-stu-id="71dfc-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="71dfc-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="71dfc-124">previewImageUrl</span></span>       | <span data-ttu-id="71dfc-125">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-125">String</span></span>        | <span data-ttu-id="71dfc-126">Uma URL que leva à imagem de visualização do item.</span><span class="sxs-lookup"><span data-stu-id="71dfc-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="71dfc-127">previewText</span><span class="sxs-lookup"><span data-stu-id="71dfc-127">previewText</span></span>           | <span data-ttu-id="71dfc-128">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-128">String</span></span>        | <span data-ttu-id="71dfc-129">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="71dfc-129">A preview text for the item.</span></span> |
| <span data-ttu-id="71dfc-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="71dfc-130">containerWebUrl</span></span>       | <span data-ttu-id="71dfc-131">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-131">String</span></span>        | <span data-ttu-id="71dfc-132">Um caminho que conduz à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="71dfc-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="71dfc-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="71dfc-133">containerDisplayName</span></span>  | <span data-ttu-id="71dfc-134">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-134">String</span></span>        | <span data-ttu-id="71dfc-135">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="71dfc-135">A string describing where the item is stored.</span></span> <span data-ttu-id="71dfc-136">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive que armazena o item.</span><span class="sxs-lookup"><span data-stu-id="71dfc-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="71dfc-137">containerType</span><span class="sxs-lookup"><span data-stu-id="71dfc-137">containerType</span></span>         | <span data-ttu-id="71dfc-138">String</span><span class="sxs-lookup"><span data-stu-id="71dfc-138">String</span></span> | <span data-ttu-id="71dfc-139">Pode ser usado para filtragem pelo tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="71dfc-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="71dfc-140">Como site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="71dfc-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="71dfc-141">Valores de propriedade Type</span><span class="sxs-lookup"><span data-stu-id="71dfc-141">Type property values</span></span>
-   <span data-ttu-id="71dfc-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="71dfc-142">PowerPoint</span></span>
-   <span data-ttu-id="71dfc-143">Word</span><span class="sxs-lookup"><span data-stu-id="71dfc-143">Word</span></span>
-   <span data-ttu-id="71dfc-144">Excel</span><span class="sxs-lookup"><span data-stu-id="71dfc-144">Excel</span></span>
-   <span data-ttu-id="71dfc-145">Documento</span><span class="sxs-lookup"><span data-stu-id="71dfc-145">Pdf</span></span>
-   <span data-ttu-id="71dfc-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="71dfc-146">OneNote</span></span>
-   <span data-ttu-id="71dfc-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="71dfc-147">OneNotePage</span></span>
-   <span data-ttu-id="71dfc-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="71dfc-148">InfoPath</span></span>
-   <span data-ttu-id="71dfc-149">Visio</span><span class="sxs-lookup"><span data-stu-id="71dfc-149">Visio</span></span>
-   <span data-ttu-id="71dfc-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="71dfc-150">Publisher</span></span>
-   <span data-ttu-id="71dfc-151">Project</span><span class="sxs-lookup"><span data-stu-id="71dfc-151">Project</span></span>
-   <span data-ttu-id="71dfc-152">Access</span><span class="sxs-lookup"><span data-stu-id="71dfc-152">Access</span></span>
-   <span data-ttu-id="71dfc-153">Email</span><span class="sxs-lookup"><span data-stu-id="71dfc-153">Mail</span></span>
-   <span data-ttu-id="71dfc-154">Limit</span><span class="sxs-lookup"><span data-stu-id="71dfc-154">Csv</span></span>
-   <span data-ttu-id="71dfc-155">Arquivo</span><span class="sxs-lookup"><span data-stu-id="71dfc-155">Archive</span></span>
-   <span data-ttu-id="71dfc-156">XPS</span><span class="sxs-lookup"><span data-stu-id="71dfc-156">Xps</span></span>
-   <span data-ttu-id="71dfc-157">Áudio</span><span class="sxs-lookup"><span data-stu-id="71dfc-157">Audio</span></span>
-   <span data-ttu-id="71dfc-158">Vídeo</span><span class="sxs-lookup"><span data-stu-id="71dfc-158">Video</span></span>
-   <span data-ttu-id="71dfc-159">Image</span><span class="sxs-lookup"><span data-stu-id="71dfc-159">Image</span></span>
-   <span data-ttu-id="71dfc-160">Web</span><span class="sxs-lookup"><span data-stu-id="71dfc-160">Web</span></span>
-   <span data-ttu-id="71dfc-161">Texto</span><span class="sxs-lookup"><span data-stu-id="71dfc-161">Text</span></span>
-   <span data-ttu-id="71dfc-162">Xml</span><span class="sxs-lookup"><span data-stu-id="71dfc-162">Xml</span></span>
-   <span data-ttu-id="71dfc-163">História</span><span class="sxs-lookup"><span data-stu-id="71dfc-163">Story</span></span>
-   <span data-ttu-id="71dfc-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="71dfc-164">ExternalContent</span></span>
-   <span data-ttu-id="71dfc-165">Folder</span><span class="sxs-lookup"><span data-stu-id="71dfc-165">Folder</span></span>
-   <span data-ttu-id="71dfc-166">Outros</span><span class="sxs-lookup"><span data-stu-id="71dfc-166">Other</span></span>

<span data-ttu-id="71dfc-167">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="71dfc-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="71dfc-168">valores da Propriedade ContainerType</span><span class="sxs-lookup"><span data-stu-id="71dfc-168">containerType property values</span></span>
<span data-ttu-id="71dfc-169">Os tipos com suporte podem diferir com base nos contêineres dos quais a [percepção](insights.md) retorna arquivos.</span><span class="sxs-lookup"><span data-stu-id="71dfc-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="71dfc-170">Por exemplo, somente a percepção [compartilhada](insights-shared.md) retorna arquivos de "Dropbox", "box" e "GDrive".</span><span class="sxs-lookup"><span data-stu-id="71dfc-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="71dfc-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="71dfc-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="71dfc-172">Site</span><span class="sxs-lookup"><span data-stu-id="71dfc-172">Site</span></span>
-   <span data-ttu-id="71dfc-173">Email</span><span class="sxs-lookup"><span data-stu-id="71dfc-173">Mail</span></span>
-   <span data-ttu-id="71dfc-174">DropBox</span><span class="sxs-lookup"><span data-stu-id="71dfc-174">DropBox</span></span>
-   <span data-ttu-id="71dfc-175">Caixa</span><span class="sxs-lookup"><span data-stu-id="71dfc-175">Box</span></span>
-   <span data-ttu-id="71dfc-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="71dfc-176">GDrive</span></span>

<span data-ttu-id="71dfc-177">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="71dfc-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
