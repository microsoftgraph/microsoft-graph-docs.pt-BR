---
title: tipo de recurso workbookWorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2f51b8a19992739d4659b41577826d5a3b024972
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019408"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="25d99-103">tipo de recurso workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="25d99-103">workbookWorksheetProtection resource type</span></span>

<span data-ttu-id="25d99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d99-105">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="25d99-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="25d99-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="25d99-106">Methods</span></span>

| <span data-ttu-id="25d99-107">Método</span><span class="sxs-lookup"><span data-stu-id="25d99-107">Method</span></span>           | <span data-ttu-id="25d99-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="25d99-108">Return Type</span></span>    |<span data-ttu-id="25d99-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="25d99-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25d99-110">Obter workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="25d99-110">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="25d99-111">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="25d99-111">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="25d99-112">Leia as propriedades e os relacionamentos do objeto workbookWorksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="25d99-112">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="25d99-113">Protect</span><span class="sxs-lookup"><span data-stu-id="25d99-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="25d99-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25d99-114">None</span></span>|<span data-ttu-id="25d99-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="25d99-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="25d99-117">Unprotect</span><span class="sxs-lookup"><span data-stu-id="25d99-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="25d99-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25d99-118">None</span></span>|<span data-ttu-id="25d99-119">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="25d99-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="25d99-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25d99-120">Properties</span></span>
| <span data-ttu-id="25d99-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25d99-121">Property</span></span>     | <span data-ttu-id="25d99-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="25d99-122">Type</span></span>   |<span data-ttu-id="25d99-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="25d99-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25d99-124">options</span><span class="sxs-lookup"><span data-stu-id="25d99-124">options</span></span>|[<span data-ttu-id="25d99-125">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="25d99-125">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="25d99-126">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="25d99-126">Sheet protection options.</span></span> <span data-ttu-id="25d99-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d99-127">Read-only.</span></span>|
|<span data-ttu-id="25d99-128">protected</span><span class="sxs-lookup"><span data-stu-id="25d99-128">protected</span></span>|<span data-ttu-id="25d99-129">booliano</span><span class="sxs-lookup"><span data-stu-id="25d99-129">boolean</span></span>|<span data-ttu-id="25d99-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d99-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25d99-132">Relações</span><span class="sxs-lookup"><span data-stu-id="25d99-132">Relationships</span></span>
<span data-ttu-id="25d99-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25d99-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25d99-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25d99-134">JSON representation</span></span>

<span data-ttu-id="25d99-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25d99-135">Here is a JSON representation of the resource.</span></span>

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


