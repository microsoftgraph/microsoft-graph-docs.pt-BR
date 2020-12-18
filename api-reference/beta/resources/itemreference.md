---
author: JeremyKelley
description: O recurso ItemReference proporciona as informações necessárias para enviar um DriveItem pela API.
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sharepoint
ms.openlocfilehash: 52cf21a4bb6d387da2c50a7ad28ab49c1b9e70ea
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714330"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="1c5f7-103">Tipo de recurso ItemReference</span><span class="sxs-lookup"><span data-stu-id="1c5f7-103">ItemReference resource type</span></span>

<span data-ttu-id="1c5f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c5f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c5f7-105">O recurso de **referência** fornece as informações necessárias para lidar com o [driveItem](driveitem.md) por meio da API.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-105">The **ItemReference** resource provides information necessary to address a [driveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c5f7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c5f7-106">JSON representation</span></span>

<span data-ttu-id="1c5f7-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1c5f7-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1c5f7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c5f7-108">Properties</span></span>

| <span data-ttu-id="1c5f7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c5f7-109">Property</span></span>      | <span data-ttu-id="1c5f7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c5f7-110">Type</span></span>              | <span data-ttu-id="1c5f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c5f7-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="1c5f7-112">driveId</span><span class="sxs-lookup"><span data-stu-id="1c5f7-112">driveId</span></span>       | <span data-ttu-id="1c5f7-113">String</span><span class="sxs-lookup"><span data-stu-id="1c5f7-113">String</span></span>            | <span data-ttu-id="1c5f7-p101">O identificador exclusivo da instância da unidade que contém o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="1c5f7-116">driveType</span><span class="sxs-lookup"><span data-stu-id="1c5f7-116">driveType</span></span>     | <span data-ttu-id="1c5f7-117">String</span><span class="sxs-lookup"><span data-stu-id="1c5f7-117">String</span></span>            | <span data-ttu-id="1c5f7-118">Identifica o tipo de unidade.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-118">Identifies the type of drive.</span></span> <span data-ttu-id="1c5f7-119">Consulte o recurso [unidade][] para obter os valores.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="1c5f7-120">id</span><span class="sxs-lookup"><span data-stu-id="1c5f7-120">id</span></span>            | <span data-ttu-id="1c5f7-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c5f7-121">String</span></span>            | <span data-ttu-id="1c5f7-p103">Identificador exclusivo do item na unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="1c5f7-124">nome</span><span class="sxs-lookup"><span data-stu-id="1c5f7-124">name</span></span>          | <span data-ttu-id="1c5f7-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c5f7-125">String</span></span>            | <span data-ttu-id="1c5f7-p104">O nome do item ao qual se faz referência. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="1c5f7-128">caminho</span><span class="sxs-lookup"><span data-stu-id="1c5f7-128">path</span></span>          | <span data-ttu-id="1c5f7-129">String</span><span class="sxs-lookup"><span data-stu-id="1c5f7-129">String</span></span>            | <span data-ttu-id="1c5f7-p105">Caminho que pode ser usado para navegar até o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="1c5f7-132">shareId</span><span class="sxs-lookup"><span data-stu-id="1c5f7-132">shareId</span></span>       | <span data-ttu-id="1c5f7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c5f7-133">String</span></span>            | <span data-ttu-id="1c5f7-134">Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="1c5f7-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="1c5f7-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="1c5f7-135">sharepointIds</span></span> | <span data-ttu-id="1c5f7-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="1c5f7-136">[sharepointIds][]</span></span> | <span data-ttu-id="1c5f7-p106">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="1c5f7-139">siteId</span><span class="sxs-lookup"><span data-stu-id="1c5f7-139">siteId</span></span>        | <span data-ttu-id="1c5f7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c5f7-140">String</span></span>            | <span data-ttu-id="1c5f7-141">Para o OneDrive for Business e o SharePoint, essa propriedade representa a ID do site que contém a biblioteca de documentos pai do recurso driveItem.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-141">For OneDrive for Business and SharePoint, this property represents the ID of the site that contains the parent document library of the driveItem resource.</span></span> <span data-ttu-id="1c5f7-142">O valor é o mesmo que a propriedade ID do recurso [site][] .</span><span class="sxs-lookup"><span data-stu-id="1c5f7-142">The value is the same as the id property of that [site][] resource.</span></span> <span data-ttu-id="1c5f7-143">É uma [cadeia de caracteres opaca que consiste em três identificadores](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true#id-property) do site.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-143">It is an [opaque string that consists of three identifiers](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true#id-property) of the site.</span></span> <br><span data-ttu-id="1c5f7-144">Para o OneDrive, essa propriedade não é preenchida.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-144">For OneDrive, this property is not populated.</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md
[site]: ../resources/site.md

## <a name="remarks"></a><span data-ttu-id="1c5f7-149">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c5f7-149">Remarks</span></span>

<span data-ttu-id="1c5f7-150">Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:</span><span class="sxs-lookup"><span data-stu-id="1c5f7-150">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="1c5f7-151">O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-151">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="1c5f7-152">Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.</span><span class="sxs-lookup"><span data-stu-id="1c5f7-152">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->


