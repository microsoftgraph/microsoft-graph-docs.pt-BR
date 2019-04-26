---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c92c02b9c5e2409ad3036bbc34c41588161ae79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345397"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="57d50-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="57d50-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="57d50-104">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="57d50-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="57d50-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="57d50-105">Methods</span></span>

| <span data-ttu-id="57d50-106">Método</span><span class="sxs-lookup"><span data-stu-id="57d50-106">Method</span></span>           | <span data-ttu-id="57d50-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57d50-107">Return Type</span></span>    |<span data-ttu-id="57d50-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="57d50-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="57d50-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="57d50-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="57d50-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="57d50-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="57d50-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="57d50-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="57d50-112">Protect</span><span class="sxs-lookup"><span data-stu-id="57d50-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="57d50-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57d50-113">None</span></span>|<span data-ttu-id="57d50-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="57d50-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="57d50-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="57d50-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="57d50-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57d50-117">None</span></span>|<span data-ttu-id="57d50-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="57d50-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="57d50-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57d50-119">Properties</span></span>
| <span data-ttu-id="57d50-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57d50-120">Property</span></span>     | <span data-ttu-id="57d50-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="57d50-121">Type</span></span>   |<span data-ttu-id="57d50-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="57d50-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57d50-123">options</span><span class="sxs-lookup"><span data-stu-id="57d50-123">options</span></span>|[<span data-ttu-id="57d50-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="57d50-124">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="57d50-125">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="57d50-125">Sheet protection options.</span></span> <span data-ttu-id="57d50-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57d50-126">Read-only.</span></span>|
|<span data-ttu-id="57d50-127">protected</span><span class="sxs-lookup"><span data-stu-id="57d50-127">protected</span></span>|<span data-ttu-id="57d50-128">booliano</span><span class="sxs-lookup"><span data-stu-id="57d50-128">boolean</span></span>|<span data-ttu-id="57d50-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57d50-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57d50-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57d50-131">JSON representation</span></span>

<span data-ttu-id="57d50-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57d50-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
