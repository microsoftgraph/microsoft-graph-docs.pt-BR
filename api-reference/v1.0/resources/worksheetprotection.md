---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8bb91dae367f9f9c95465aed0f8c71a26aaddd1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014998"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="ceeb9-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="ceeb9-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="ceeb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceeb9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ceeb9-105">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="ceeb9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ceeb9-106">Methods</span></span>

| <span data-ttu-id="ceeb9-107">Método</span><span class="sxs-lookup"><span data-stu-id="ceeb9-107">Method</span></span>           | <span data-ttu-id="ceeb9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ceeb9-108">Return Type</span></span>    |<span data-ttu-id="ceeb9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceeb9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ceeb9-110">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="ceeb9-110">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="ceeb9-111">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="ceeb9-111">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="ceeb9-112">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-112">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="ceeb9-113">Protect</span><span class="sxs-lookup"><span data-stu-id="ceeb9-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="ceeb9-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ceeb9-114">None</span></span>|<span data-ttu-id="ceeb9-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="ceeb9-117">Unprotect</span><span class="sxs-lookup"><span data-stu-id="ceeb9-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="ceeb9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ceeb9-118">None</span></span>|<span data-ttu-id="ceeb9-119">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="ceeb9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ceeb9-120">Properties</span></span>
| <span data-ttu-id="ceeb9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ceeb9-121">Property</span></span>     | <span data-ttu-id="ceeb9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceeb9-122">Type</span></span>   |<span data-ttu-id="ceeb9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceeb9-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceeb9-124">options</span><span class="sxs-lookup"><span data-stu-id="ceeb9-124">options</span></span>|[<span data-ttu-id="ceeb9-125">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="ceeb9-125">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="ceeb9-126">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-126">Sheet protection options.</span></span> <span data-ttu-id="ceeb9-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-127">Read-only.</span></span>|
|<span data-ttu-id="ceeb9-128">protected</span><span class="sxs-lookup"><span data-stu-id="ceeb9-128">protected</span></span>|<span data-ttu-id="ceeb9-129">booliano</span><span class="sxs-lookup"><span data-stu-id="ceeb9-129">boolean</span></span>|<span data-ttu-id="ceeb9-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ceeb9-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ceeb9-132">JSON representation</span></span>

<span data-ttu-id="ceeb9-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ceeb9-133">Here is a JSON representation of the resource.</span></span>

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

