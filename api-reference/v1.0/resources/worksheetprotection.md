---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 805c3b53a60495ebd50a230a83e3ce1272cacf4d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446664"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="f555d-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f555d-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="f555d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f555d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f555d-105">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="f555d-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="f555d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f555d-106">Methods</span></span>

| <span data-ttu-id="f555d-107">Método</span><span class="sxs-lookup"><span data-stu-id="f555d-107">Method</span></span>           | <span data-ttu-id="f555d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f555d-108">Return Type</span></span>    |<span data-ttu-id="f555d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f555d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f555d-110">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f555d-110">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="f555d-111">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f555d-111">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="f555d-112">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="f555d-112">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="f555d-113">Protect</span><span class="sxs-lookup"><span data-stu-id="f555d-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="f555d-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f555d-114">None</span></span>|<span data-ttu-id="f555d-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="f555d-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="f555d-117">Unprotect</span><span class="sxs-lookup"><span data-stu-id="f555d-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="f555d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f555d-118">None</span></span>|<span data-ttu-id="f555d-119">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="f555d-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="f555d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f555d-120">Properties</span></span>
| <span data-ttu-id="f555d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f555d-121">Property</span></span>     | <span data-ttu-id="f555d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f555d-122">Type</span></span>   |<span data-ttu-id="f555d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f555d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f555d-124">options</span><span class="sxs-lookup"><span data-stu-id="f555d-124">options</span></span>|[<span data-ttu-id="f555d-125">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="f555d-125">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="f555d-126">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="f555d-126">Sheet protection options.</span></span> <span data-ttu-id="f555d-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f555d-127">Read-only.</span></span>|
|<span data-ttu-id="f555d-128">protected</span><span class="sxs-lookup"><span data-stu-id="f555d-128">protected</span></span>|<span data-ttu-id="f555d-129">booliano</span><span class="sxs-lookup"><span data-stu-id="f555d-129">boolean</span></span>|<span data-ttu-id="f555d-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f555d-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f555d-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f555d-132">JSON representation</span></span>

<span data-ttu-id="f555d-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f555d-133">Here is a JSON representation of the resource.</span></span>

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
