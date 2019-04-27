---
title: tipo de recurso workbookWorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e4a2f3130c71df35b1106d1a342004cfc6fdf25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348478"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="703c6-103">tipo de recurso workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="703c6-103">workbookWorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="703c6-104">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="703c6-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="703c6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="703c6-105">Methods</span></span>

| <span data-ttu-id="703c6-106">Método</span><span class="sxs-lookup"><span data-stu-id="703c6-106">Method</span></span>           | <span data-ttu-id="703c6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="703c6-107">Return Type</span></span>    |<span data-ttu-id="703c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="703c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="703c6-109">Obter workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="703c6-109">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="703c6-110">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="703c6-110">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="703c6-111">Leia as propriedades e os relacionamentos do objeto workbookWorksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="703c6-111">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="703c6-112">Protect</span><span class="sxs-lookup"><span data-stu-id="703c6-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="703c6-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="703c6-113">None</span></span>|<span data-ttu-id="703c6-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="703c6-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="703c6-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="703c6-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="703c6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="703c6-117">None</span></span>|<span data-ttu-id="703c6-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="703c6-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="703c6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="703c6-119">Properties</span></span>
| <span data-ttu-id="703c6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="703c6-120">Property</span></span>     | <span data-ttu-id="703c6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="703c6-121">Type</span></span>   |<span data-ttu-id="703c6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="703c6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="703c6-123">options</span><span class="sxs-lookup"><span data-stu-id="703c6-123">options</span></span>|[<span data-ttu-id="703c6-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="703c6-124">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="703c6-125">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="703c6-125">Sheet protection options.</span></span> <span data-ttu-id="703c6-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="703c6-126">Read-only.</span></span>|
|<span data-ttu-id="703c6-127">protected</span><span class="sxs-lookup"><span data-stu-id="703c6-127">protected</span></span>|<span data-ttu-id="703c6-128">booliano</span><span class="sxs-lookup"><span data-stu-id="703c6-128">boolean</span></span>|<span data-ttu-id="703c6-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="703c6-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="703c6-131">Relações</span><span class="sxs-lookup"><span data-stu-id="703c6-131">Relationships</span></span>
<span data-ttu-id="703c6-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="703c6-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="703c6-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="703c6-133">JSON representation</span></span>

<span data-ttu-id="703c6-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="703c6-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
