---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: O recurso ItemReference proporciona as informações necessárias para enviar um DriveItem pela API.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a13fb5a3606b72c96a15317a9a7b1d5844184f4c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009223"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="b2e39-103">Tipo de recurso ItemReference</span><span class="sxs-lookup"><span data-stu-id="b2e39-103">ItemReference resource type</span></span>

<span data-ttu-id="b2e39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2e39-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2e39-105">O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.</span><span class="sxs-lookup"><span data-stu-id="b2e39-105">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e39-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2e39-106">JSON representation</span></span>

<span data-ttu-id="b2e39-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b2e39-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b2e39-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2e39-108">Properties</span></span>

| <span data-ttu-id="b2e39-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2e39-109">Property</span></span>      | <span data-ttu-id="b2e39-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2e39-110">Type</span></span>              | <span data-ttu-id="b2e39-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2e39-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="b2e39-112">driveId</span><span class="sxs-lookup"><span data-stu-id="b2e39-112">driveId</span></span>       | <span data-ttu-id="b2e39-113">String</span><span class="sxs-lookup"><span data-stu-id="b2e39-113">String</span></span>            | <span data-ttu-id="b2e39-p101">O identificador exclusivo da instância da unidade que contém o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e39-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="b2e39-116">driveType</span><span class="sxs-lookup"><span data-stu-id="b2e39-116">driveType</span></span>     | <span data-ttu-id="b2e39-117">String</span><span class="sxs-lookup"><span data-stu-id="b2e39-117">String</span></span>            | <span data-ttu-id="b2e39-118">Identifica o tipo de unidade.</span><span class="sxs-lookup"><span data-stu-id="b2e39-118">Identifies the type of drive.</span></span> <span data-ttu-id="b2e39-119">Consulte o recurso [unidade][] para obter os valores.</span><span class="sxs-lookup"><span data-stu-id="b2e39-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="b2e39-120">id</span><span class="sxs-lookup"><span data-stu-id="b2e39-120">id</span></span>            | <span data-ttu-id="b2e39-121">String</span><span class="sxs-lookup"><span data-stu-id="b2e39-121">String</span></span>            | <span data-ttu-id="b2e39-p103">Identificador exclusivo do item na unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e39-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="b2e39-124">nome</span><span class="sxs-lookup"><span data-stu-id="b2e39-124">name</span></span>          | <span data-ttu-id="b2e39-125">String</span><span class="sxs-lookup"><span data-stu-id="b2e39-125">String</span></span>            | <span data-ttu-id="b2e39-p104">O nome do item ao qual se faz referência. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e39-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="b2e39-128">caminho</span><span class="sxs-lookup"><span data-stu-id="b2e39-128">path</span></span>          | <span data-ttu-id="b2e39-129">String</span><span class="sxs-lookup"><span data-stu-id="b2e39-129">String</span></span>            | <span data-ttu-id="b2e39-p105">Caminho que pode ser usado para navegar até o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e39-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="b2e39-132">shareId</span><span class="sxs-lookup"><span data-stu-id="b2e39-132">shareId</span></span>       | <span data-ttu-id="b2e39-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2e39-133">String</span></span>            | <span data-ttu-id="b2e39-134">Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="b2e39-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="b2e39-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b2e39-135">sharepointIds</span></span> | <span data-ttu-id="b2e39-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b2e39-136">[sharepointIds][]</span></span> | <span data-ttu-id="b2e39-p106">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e39-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="b2e39-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2e39-142">Remarks</span></span>

<span data-ttu-id="b2e39-143">Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:</span><span class="sxs-lookup"><span data-stu-id="b2e39-143">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="b2e39-144">O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="b2e39-144">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="b2e39-145">Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.</span><span class="sxs-lookup"><span data-stu-id="b2e39-145">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

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

