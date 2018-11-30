---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
ms.openlocfilehash: aae92566503ce7bdb4a742c33b1a65c43937662c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005014"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="45f34-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="45f34-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="45f34-104">Representa a proteção de um objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="45f34-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="45f34-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="45f34-105">Methods</span></span>

| <span data-ttu-id="45f34-106">Método</span><span class="sxs-lookup"><span data-stu-id="45f34-106">Method</span></span>           | <span data-ttu-id="45f34-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45f34-107">Return Type</span></span>    |<span data-ttu-id="45f34-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f34-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45f34-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="45f34-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="45f34-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="45f34-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="45f34-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="45f34-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="45f34-112">Protect</span><span class="sxs-lookup"><span data-stu-id="45f34-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="45f34-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45f34-113">None</span></span>|<span data-ttu-id="45f34-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="45f34-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="45f34-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="45f34-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="45f34-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45f34-117">None</span></span>|<span data-ttu-id="45f34-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="45f34-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="45f34-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45f34-119">Properties</span></span>
| <span data-ttu-id="45f34-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45f34-120">Property</span></span>     | <span data-ttu-id="45f34-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="45f34-121">Type</span></span>   |<span data-ttu-id="45f34-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f34-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45f34-123">options</span><span class="sxs-lookup"><span data-stu-id="45f34-123">options</span></span>|[<span data-ttu-id="45f34-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="45f34-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="45f34-p102">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45f34-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="45f34-127">protected</span><span class="sxs-lookup"><span data-stu-id="45f34-127">protected</span></span>|<span data-ttu-id="45f34-128">booliano</span><span class="sxs-lookup"><span data-stu-id="45f34-128">boolean</span></span>|<span data-ttu-id="45f34-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45f34-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45f34-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45f34-131">JSON representation</span></span>

<span data-ttu-id="45f34-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45f34-132">Here is a JSON representation of the resource.</span></span>

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