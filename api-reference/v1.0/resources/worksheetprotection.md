---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9d3cbf4c03ff1e9938c7464d1501f261634ef347
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033303"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="4973c-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4973c-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="4973c-104">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="4973c-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4973c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4973c-105">Methods</span></span>

| <span data-ttu-id="4973c-106">Método</span><span class="sxs-lookup"><span data-stu-id="4973c-106">Method</span></span>           | <span data-ttu-id="4973c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4973c-107">Return Type</span></span>    |<span data-ttu-id="4973c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4973c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4973c-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4973c-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="4973c-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4973c-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="4973c-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="4973c-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="4973c-112">Protect</span><span class="sxs-lookup"><span data-stu-id="4973c-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="4973c-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4973c-113">None</span></span>|<span data-ttu-id="4973c-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="4973c-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4973c-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="4973c-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="4973c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4973c-117">None</span></span>|<span data-ttu-id="4973c-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="4973c-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4973c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4973c-119">Properties</span></span>
| <span data-ttu-id="4973c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4973c-120">Property</span></span>     | <span data-ttu-id="4973c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4973c-121">Type</span></span>   |<span data-ttu-id="4973c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4973c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4973c-123">options</span><span class="sxs-lookup"><span data-stu-id="4973c-123">options</span></span>|[<span data-ttu-id="4973c-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4973c-124">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="4973c-125">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="4973c-125">Sheet protection options.</span></span> <span data-ttu-id="4973c-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4973c-126">Read-only.</span></span>|
|<span data-ttu-id="4973c-127">protected</span><span class="sxs-lookup"><span data-stu-id="4973c-127">protected</span></span>|<span data-ttu-id="4973c-128">booliano</span><span class="sxs-lookup"><span data-stu-id="4973c-128">boolean</span></span>|<span data-ttu-id="4973c-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4973c-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4973c-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4973c-131">JSON representation</span></span>

<span data-ttu-id="4973c-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4973c-132">Here is a JSON representation of the resource.</span></span>

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
