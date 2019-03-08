---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
ms.openlocfilehash: 63155bbeb586956f539b0c28ac1f7706189b5445
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482277"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="fba2c-102">Tipo de recurso ItemReference</span><span class="sxs-lookup"><span data-stu-id="fba2c-102">ItemReference resource type</span></span>

<span data-ttu-id="fba2c-103">O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.</span><span class="sxs-lookup"><span data-stu-id="fba2c-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba2c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fba2c-104">JSON representation</span></span>

<span data-ttu-id="fba2c-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fba2c-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="fba2c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fba2c-106">Properties</span></span>

| <span data-ttu-id="fba2c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fba2c-107">Property</span></span>      | <span data-ttu-id="fba2c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fba2c-108">Type</span></span>              | <span data-ttu-id="fba2c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba2c-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="fba2c-110">driveId</span><span class="sxs-lookup"><span data-stu-id="fba2c-110">driveId</span></span>       | <span data-ttu-id="fba2c-111">String</span><span class="sxs-lookup"><span data-stu-id="fba2c-111">String</span></span>            | <span data-ttu-id="fba2c-p101">O identificador exclusivo da instância da unidade que contém o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fba2c-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="fba2c-114">driveType</span><span class="sxs-lookup"><span data-stu-id="fba2c-114">driveType</span></span>     | <span data-ttu-id="fba2c-115">String</span><span class="sxs-lookup"><span data-stu-id="fba2c-115">String</span></span>            | <span data-ttu-id="fba2c-116">Identifica o tipo de unidade.</span><span class="sxs-lookup"><span data-stu-id="fba2c-116">Identifies the type of drive.</span></span> <span data-ttu-id="fba2c-117">Consulte o recurso [unidade][] para obter os valores.</span><span class="sxs-lookup"><span data-stu-id="fba2c-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="fba2c-118">id</span><span class="sxs-lookup"><span data-stu-id="fba2c-118">id</span></span>            | <span data-ttu-id="fba2c-119">String</span><span class="sxs-lookup"><span data-stu-id="fba2c-119">String</span></span>            | <span data-ttu-id="fba2c-p103">Identificador exclusivo do item na unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fba2c-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="fba2c-122">nome</span><span class="sxs-lookup"><span data-stu-id="fba2c-122">name</span></span>          | <span data-ttu-id="fba2c-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba2c-123">String</span></span>            | <span data-ttu-id="fba2c-p104">O nome do item ao qual se faz referência. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fba2c-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="fba2c-126">caminho</span><span class="sxs-lookup"><span data-stu-id="fba2c-126">path</span></span>          | <span data-ttu-id="fba2c-127">String</span><span class="sxs-lookup"><span data-stu-id="fba2c-127">String</span></span>            | <span data-ttu-id="fba2c-p105">Caminho que pode ser usado para navegar até o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fba2c-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="fba2c-130">shareId</span><span class="sxs-lookup"><span data-stu-id="fba2c-130">shareId</span></span>       | <span data-ttu-id="fba2c-131">String</span><span class="sxs-lookup"><span data-stu-id="fba2c-131">String</span></span>            | <span data-ttu-id="fba2c-132">Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares][].</span><span class="sxs-lookup"><span data-stu-id="fba2c-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="fba2c-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="fba2c-133">sharepointIds</span></span> | <span data-ttu-id="fba2c-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="fba2c-134">[sharepointIds][]</span></span> | <span data-ttu-id="fba2c-p106">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fba2c-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="fba2c-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="fba2c-140">Remarks</span></span>

<span data-ttu-id="fba2c-141">Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:</span><span class="sxs-lookup"><span data-stu-id="fba2c-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="fba2c-142">O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="fba2c-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="fba2c-143">Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.</span><span class="sxs-lookup"><span data-stu-id="fba2c-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
