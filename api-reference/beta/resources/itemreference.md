---
author: JeremyKelley
description: O recurso ItemReference proporciona as informações necessárias para enviar um DriveItem pela API.
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4f9b061757405f284e367cc4311230c76515a086
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523048"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="701ef-103">Tipo de recurso ItemReference</span><span class="sxs-lookup"><span data-stu-id="701ef-103">ItemReference resource type</span></span>

<span data-ttu-id="701ef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="701ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="701ef-105">O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.</span><span class="sxs-lookup"><span data-stu-id="701ef-105">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="701ef-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="701ef-106">JSON representation</span></span>

<span data-ttu-id="701ef-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="701ef-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="701ef-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="701ef-108">Properties</span></span>

| <span data-ttu-id="701ef-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="701ef-109">Property</span></span>      | <span data-ttu-id="701ef-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="701ef-110">Type</span></span>              | <span data-ttu-id="701ef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="701ef-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="701ef-112">driveId</span><span class="sxs-lookup"><span data-stu-id="701ef-112">driveId</span></span>       | <span data-ttu-id="701ef-113">String</span><span class="sxs-lookup"><span data-stu-id="701ef-113">String</span></span>            | <span data-ttu-id="701ef-p101">O identificador exclusivo da instância da unidade que contém o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="701ef-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="701ef-116">driveType</span><span class="sxs-lookup"><span data-stu-id="701ef-116">driveType</span></span>     | <span data-ttu-id="701ef-117">String</span><span class="sxs-lookup"><span data-stu-id="701ef-117">String</span></span>            | <span data-ttu-id="701ef-118">Identifica o tipo de unidade.</span><span class="sxs-lookup"><span data-stu-id="701ef-118">Identifies the type of drive.</span></span> <span data-ttu-id="701ef-119">Consulte o recurso [unidade][] para obter os valores.</span><span class="sxs-lookup"><span data-stu-id="701ef-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="701ef-120">id</span><span class="sxs-lookup"><span data-stu-id="701ef-120">id</span></span>            | <span data-ttu-id="701ef-121">String</span><span class="sxs-lookup"><span data-stu-id="701ef-121">String</span></span>            | <span data-ttu-id="701ef-p103">Identificador exclusivo do item na unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="701ef-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="701ef-124">nome</span><span class="sxs-lookup"><span data-stu-id="701ef-124">name</span></span>          | <span data-ttu-id="701ef-125">String</span><span class="sxs-lookup"><span data-stu-id="701ef-125">String</span></span>            | <span data-ttu-id="701ef-p104">O nome do item ao qual se faz referência. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="701ef-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="701ef-128">caminho</span><span class="sxs-lookup"><span data-stu-id="701ef-128">path</span></span>          | <span data-ttu-id="701ef-129">String</span><span class="sxs-lookup"><span data-stu-id="701ef-129">String</span></span>            | <span data-ttu-id="701ef-p105">Caminho que pode ser usado para navegar até o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="701ef-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="701ef-132">shareId</span><span class="sxs-lookup"><span data-stu-id="701ef-132">shareId</span></span>       | <span data-ttu-id="701ef-133">String</span><span class="sxs-lookup"><span data-stu-id="701ef-133">String</span></span>            | <span data-ttu-id="701ef-134">Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="701ef-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="701ef-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="701ef-135">sharepointIds</span></span> | <span data-ttu-id="701ef-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="701ef-136">[sharepointIds][]</span></span> | <span data-ttu-id="701ef-p106">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="701ef-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="701ef-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="701ef-142">Remarks</span></span>

<span data-ttu-id="701ef-143">Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:</span><span class="sxs-lookup"><span data-stu-id="701ef-143">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="701ef-144">O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="701ef-144">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="701ef-145">Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.</span><span class="sxs-lookup"><span data-stu-id="701ef-145">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
