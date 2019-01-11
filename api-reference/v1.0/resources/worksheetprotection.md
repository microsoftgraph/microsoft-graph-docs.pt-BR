---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f0bbf3652223a532cd3d815aca832d4cfcd37171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860710"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="86128-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="86128-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="86128-104">Representa a proteção de um objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="86128-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="86128-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="86128-105">Methods</span></span>

| <span data-ttu-id="86128-106">Método</span><span class="sxs-lookup"><span data-stu-id="86128-106">Method</span></span>           | <span data-ttu-id="86128-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86128-107">Return Type</span></span>    |<span data-ttu-id="86128-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="86128-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86128-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="86128-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="86128-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="86128-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="86128-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="86128-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="86128-112">Protect</span><span class="sxs-lookup"><span data-stu-id="86128-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="86128-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86128-113">None</span></span>|<span data-ttu-id="86128-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="86128-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="86128-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="86128-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="86128-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86128-117">None</span></span>|<span data-ttu-id="86128-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="86128-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="86128-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86128-119">Properties</span></span>
| <span data-ttu-id="86128-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86128-120">Property</span></span>     | <span data-ttu-id="86128-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="86128-121">Type</span></span>   |<span data-ttu-id="86128-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="86128-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86128-123">options</span><span class="sxs-lookup"><span data-stu-id="86128-123">options</span></span>|[<span data-ttu-id="86128-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="86128-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="86128-p102">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86128-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="86128-127">protected</span><span class="sxs-lookup"><span data-stu-id="86128-127">protected</span></span>|<span data-ttu-id="86128-128">booliano</span><span class="sxs-lookup"><span data-stu-id="86128-128">boolean</span></span>|<span data-ttu-id="86128-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86128-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86128-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86128-131">JSON representation</span></span>

<span data-ttu-id="86128-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86128-132">Here is a JSON representation of the resource.</span></span>

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
