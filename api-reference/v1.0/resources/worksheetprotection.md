---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a719d1be9f21edf1bef82d2aa058b45bbf2df8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463611"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="455bb-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="455bb-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="455bb-104">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="455bb-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="455bb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="455bb-105">Methods</span></span>

| <span data-ttu-id="455bb-106">Método</span><span class="sxs-lookup"><span data-stu-id="455bb-106">Method</span></span>           | <span data-ttu-id="455bb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="455bb-107">Return Type</span></span>    |<span data-ttu-id="455bb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="455bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="455bb-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="455bb-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="455bb-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="455bb-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="455bb-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="455bb-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="455bb-112">Protect</span><span class="sxs-lookup"><span data-stu-id="455bb-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="455bb-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="455bb-113">None</span></span>|<span data-ttu-id="455bb-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="455bb-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="455bb-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="455bb-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="455bb-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="455bb-117">None</span></span>|<span data-ttu-id="455bb-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="455bb-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="455bb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="455bb-119">Properties</span></span>
| <span data-ttu-id="455bb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="455bb-120">Property</span></span>     | <span data-ttu-id="455bb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="455bb-121">Type</span></span>   |<span data-ttu-id="455bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="455bb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="455bb-123">options</span><span class="sxs-lookup"><span data-stu-id="455bb-123">options</span></span>|[<span data-ttu-id="455bb-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="455bb-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="455bb-125">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="455bb-125">Sheet protection options.</span></span> <span data-ttu-id="455bb-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="455bb-126">Read-only.</span></span>|
|<span data-ttu-id="455bb-127">protected</span><span class="sxs-lookup"><span data-stu-id="455bb-127">protected</span></span>|<span data-ttu-id="455bb-128">booliano</span><span class="sxs-lookup"><span data-stu-id="455bb-128">boolean</span></span>|<span data-ttu-id="455bb-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="455bb-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="455bb-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="455bb-131">JSON representation</span></span>

<span data-ttu-id="455bb-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="455bb-132">Here is a JSON representation of the resource.</span></span>

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
