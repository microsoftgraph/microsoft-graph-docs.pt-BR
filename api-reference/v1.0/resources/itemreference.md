---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: O recurso ItemReference proporciona as informações necessárias para enviar um DriveItem pela API.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f7d8f6d524b605b544785b0379a273d4c022c9c9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036523"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="d3e9c-103">Tipo de recurso ItemReference</span><span class="sxs-lookup"><span data-stu-id="d3e9c-103">ItemReference resource type</span></span>

<span data-ttu-id="d3e9c-104">O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-104">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3e9c-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3e9c-105">JSON representation</span></span>

<span data-ttu-id="d3e9c-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d3e9c-106">Here is a JSON representation of the resource</span></span>

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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="d3e9c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3e9c-107">Properties</span></span>

| <span data-ttu-id="d3e9c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3e9c-108">Property</span></span>      | <span data-ttu-id="d3e9c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3e9c-109">Type</span></span>              | <span data-ttu-id="d3e9c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e9c-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="d3e9c-111">driveId</span><span class="sxs-lookup"><span data-stu-id="d3e9c-111">driveId</span></span>       | <span data-ttu-id="d3e9c-112">String</span><span class="sxs-lookup"><span data-stu-id="d3e9c-112">String</span></span>            | <span data-ttu-id="d3e9c-p101">O identificador exclusivo da instância da unidade que contém o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="d3e9c-115">driveType</span><span class="sxs-lookup"><span data-stu-id="d3e9c-115">driveType</span></span>     | <span data-ttu-id="d3e9c-116">String</span><span class="sxs-lookup"><span data-stu-id="d3e9c-116">String</span></span>            | <span data-ttu-id="d3e9c-117">Identifica o tipo de unidade.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-117">Identifies the type of drive.</span></span> <span data-ttu-id="d3e9c-118">Consulte o recurso [unidade][] para obter os valores.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-118">See [drive][] resource for values.</span></span>
| <span data-ttu-id="d3e9c-119">id</span><span class="sxs-lookup"><span data-stu-id="d3e9c-119">id</span></span>            | <span data-ttu-id="d3e9c-120">String</span><span class="sxs-lookup"><span data-stu-id="d3e9c-120">String</span></span>            | <span data-ttu-id="d3e9c-p103">Identificador exclusivo do item na unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="d3e9c-123">name</span><span class="sxs-lookup"><span data-stu-id="d3e9c-123">name</span></span>          | <span data-ttu-id="d3e9c-124">String</span><span class="sxs-lookup"><span data-stu-id="d3e9c-124">String</span></span>            | <span data-ttu-id="d3e9c-p104">O nome do item ao qual se faz referência. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="d3e9c-127">caminho</span><span class="sxs-lookup"><span data-stu-id="d3e9c-127">path</span></span>          | <span data-ttu-id="d3e9c-128">String</span><span class="sxs-lookup"><span data-stu-id="d3e9c-128">String</span></span>            | <span data-ttu-id="d3e9c-p105">Caminho que pode ser usado para navegar até o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="d3e9c-131">shareId</span><span class="sxs-lookup"><span data-stu-id="d3e9c-131">shareId</span></span>       | <span data-ttu-id="d3e9c-132">String</span><span class="sxs-lookup"><span data-stu-id="d3e9c-132">String</span></span>            | <span data-ttu-id="d3e9c-133">Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="d3e9c-133">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="d3e9c-134">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="d3e9c-134">sharepointIds</span></span> | <span data-ttu-id="d3e9c-135">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="d3e9c-135">[sharepointIds][]</span></span> | <span data-ttu-id="d3e9c-p106">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="d3e9c-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="d3e9c-141">Remarks</span></span>

<span data-ttu-id="d3e9c-142">Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:</span><span class="sxs-lookup"><span data-stu-id="d3e9c-142">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="d3e9c-143">O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-143">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="d3e9c-144">Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.</span><span class="sxs-lookup"><span data-stu-id="d3e9c-144">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->
