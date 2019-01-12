---
title: tipo de recurso de resourceVisualization
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8426d13968e5bea929c8e26f71346fa554a5242
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990653"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="9d8d3-103">tipo de recurso de resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="9d8d3-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="9d8d3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d8d3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d8d3-106">Tipo complexo que contém propriedades de [ideias](insights.md).</span><span class="sxs-lookup"><span data-stu-id="9d8d3-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d8d3-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d8d3-107">JSON representation</span></span>

<span data-ttu-id="9d8d3-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9d8d3-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="9d8d3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d8d3-109">Properties</span></span>

| <span data-ttu-id="9d8d3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d8d3-110">Property</span></span>              | <span data-ttu-id="9d8d3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d8d3-111">Type</span></span>          | <span data-ttu-id="9d8d3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d8d3-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="9d8d3-113">title</span><span class="sxs-lookup"><span data-stu-id="9d8d3-113">title</span></span>                 | <span data-ttu-id="9d8d3-114">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-114">String</span></span>        | <span data-ttu-id="9d8d3-115">Texto do título do item.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-115">The item's title text.</span></span>               |
| <span data-ttu-id="9d8d3-116">type</span><span class="sxs-lookup"><span data-stu-id="9d8d3-116">type</span></span>              | <span data-ttu-id="9d8d3-117">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-117">String</span></span>        | <span data-ttu-id="9d8d3-118">Tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-118">The item's media type.</span></span> <span data-ttu-id="9d8d3-119">Pode ser usado para filtrar para um arquivo específico com base em um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="9d8d3-120">Veja abaixo tipos suportados.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-120">See below for supported types.</span></span> |
| <span data-ttu-id="9d8d3-121">mediaType</span><span class="sxs-lookup"><span data-stu-id="9d8d3-121">mediaType</span></span>             | <span data-ttu-id="9d8d3-122">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-122">String</span></span>        | <span data-ttu-id="9d8d3-123">Tipo de mídia do item.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-123">The item's media type.</span></span> <span data-ttu-id="9d8d3-124">Pode ser usado para filtragem para um tipo específico de arquivo com base em tipos de Mime de mídia IANA suportados.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="9d8d3-125">Observe que nem todos os tipos de Mime de mídia são suportados.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="9d8d3-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="9d8d3-126">previewImageUrl</span></span>       | <span data-ttu-id="9d8d3-127">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-127">String</span></span>        | <span data-ttu-id="9d8d3-128">Uma URL, levando a imagem de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="9d8d3-129">previewText</span><span class="sxs-lookup"><span data-stu-id="9d8d3-129">previewText</span></span>           | <span data-ttu-id="9d8d3-130">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-130">String</span></span>        | <span data-ttu-id="9d8d3-131">Um texto de visualização para o item.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-131">A preview text for the item.</span></span> |
| <span data-ttu-id="9d8d3-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="9d8d3-132">containerWebUrl</span></span>       | <span data-ttu-id="9d8d3-133">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-133">String</span></span>        | <span data-ttu-id="9d8d3-134">Um caminho que leva à pasta na qual o item está armazenado.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="9d8d3-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d8d3-135">containerDisplayName</span></span>  | <span data-ttu-id="9d8d3-136">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-136">String</span></span>        | <span data-ttu-id="9d8d3-137">Uma cadeia de caracteres que descreve onde o item é armazenado.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-137">A string describing where the item is stored.</span></span> <span data-ttu-id="9d8d3-138">Por exemplo, o nome de um site do SharePoint ou o nome de usuário que identifica o proprietário do OneDrive armazenar o item.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="9d8d3-139">containerType</span><span class="sxs-lookup"><span data-stu-id="9d8d3-139">containerType</span></span>         | <span data-ttu-id="9d8d3-140">String</span><span class="sxs-lookup"><span data-stu-id="9d8d3-140">String</span></span> | <span data-ttu-id="9d8d3-141">Pode ser usado para filtrar por tipo de contêiner no qual o arquivo está armazenado.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="9d8d3-142">Como o Site ou OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="9d8d3-143">Valores de tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="9d8d3-143">Type property values</span></span>
-   <span data-ttu-id="9d8d3-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="9d8d3-144">PowerPoint</span></span>
-   <span data-ttu-id="9d8d3-145">Word</span><span class="sxs-lookup"><span data-stu-id="9d8d3-145">Word</span></span>
-   <span data-ttu-id="9d8d3-146">Excel</span><span class="sxs-lookup"><span data-stu-id="9d8d3-146">Excel</span></span>
-   <span data-ttu-id="9d8d3-147">PDF</span><span class="sxs-lookup"><span data-stu-id="9d8d3-147">Pdf</span></span>
-   <span data-ttu-id="9d8d3-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="9d8d3-148">OneNote</span></span>
-   <span data-ttu-id="9d8d3-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="9d8d3-149">OneNotePage</span></span>
-   <span data-ttu-id="9d8d3-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="9d8d3-150">InfoPath</span></span>
-   <span data-ttu-id="9d8d3-151">Visio</span><span class="sxs-lookup"><span data-stu-id="9d8d3-151">Visio</span></span>
-   <span data-ttu-id="9d8d3-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="9d8d3-152">Publisher</span></span>
-   <span data-ttu-id="9d8d3-153">Project</span><span class="sxs-lookup"><span data-stu-id="9d8d3-153">Project</span></span>
-   <span data-ttu-id="9d8d3-154">Access</span><span class="sxs-lookup"><span data-stu-id="9d8d3-154">Access</span></span>
-   <span data-ttu-id="9d8d3-155">Email</span><span class="sxs-lookup"><span data-stu-id="9d8d3-155">Mail</span></span>
-   <span data-ttu-id="9d8d3-156">CSV</span><span class="sxs-lookup"><span data-stu-id="9d8d3-156">Csv</span></span>
-   <span data-ttu-id="9d8d3-157">Arquivo morto</span><span class="sxs-lookup"><span data-stu-id="9d8d3-157">Archive</span></span>
-   <span data-ttu-id="9d8d3-158">XPS</span><span class="sxs-lookup"><span data-stu-id="9d8d3-158">Xps</span></span>
-   <span data-ttu-id="9d8d3-159">Áudio</span><span class="sxs-lookup"><span data-stu-id="9d8d3-159">Audio</span></span>
-   <span data-ttu-id="9d8d3-160">Vídeo</span><span class="sxs-lookup"><span data-stu-id="9d8d3-160">Video</span></span>
-   <span data-ttu-id="9d8d3-161">Image</span><span class="sxs-lookup"><span data-stu-id="9d8d3-161">Image</span></span>
-   <span data-ttu-id="9d8d3-162">Web</span><span class="sxs-lookup"><span data-stu-id="9d8d3-162">Web</span></span>
-   <span data-ttu-id="9d8d3-163">Texto</span><span class="sxs-lookup"><span data-stu-id="9d8d3-163">Text</span></span>
-   <span data-ttu-id="9d8d3-164">Xml</span><span class="sxs-lookup"><span data-stu-id="9d8d3-164">Xml</span></span>
-   <span data-ttu-id="9d8d3-165">Story</span><span class="sxs-lookup"><span data-stu-id="9d8d3-165">Story</span></span>
-   <span data-ttu-id="9d8d3-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="9d8d3-166">ExternalContent</span></span>
-   <span data-ttu-id="9d8d3-167">Folder</span><span class="sxs-lookup"><span data-stu-id="9d8d3-167">Folder</span></span>
-   <span data-ttu-id="9d8d3-168">Outros</span><span class="sxs-lookup"><span data-stu-id="9d8d3-168">Other</span></span>

<span data-ttu-id="9d8d3-169">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="9d8d3-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="9d8d3-170">valores de propriedade containerType</span><span class="sxs-lookup"><span data-stu-id="9d8d3-170">containerType property values</span></span>
<span data-ttu-id="9d8d3-171">Os tipos suportados podem variar, dependendo em contêineres do qual a [percepção](insights.md) retorna os arquivos.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="9d8d3-172">Por exemplo, apenas o insight [compartilhados](insights-shared.md) retorna arquivos do 'Recados', 'Caixa' e 'GDrive'.</span><span class="sxs-lookup"><span data-stu-id="9d8d3-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="9d8d3-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="9d8d3-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="9d8d3-174">Site</span><span class="sxs-lookup"><span data-stu-id="9d8d3-174">Site</span></span>
-   <span data-ttu-id="9d8d3-175">Email</span><span class="sxs-lookup"><span data-stu-id="9d8d3-175">Mail</span></span>
-   <span data-ttu-id="9d8d3-176">Pasta de recados</span><span class="sxs-lookup"><span data-stu-id="9d8d3-176">DropBox</span></span>
-   <span data-ttu-id="9d8d3-177">Caixa</span><span class="sxs-lookup"><span data-stu-id="9d8d3-177">Box</span></span>
-   <span data-ttu-id="9d8d3-178">GDrive</span><span class="sxs-lookup"><span data-stu-id="9d8d3-178">GDrive</span></span>

<span data-ttu-id="9d8d3-179">Consulta de exemplo:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="9d8d3-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
