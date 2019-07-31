---
title: tipo de recurso workbookWorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ed6f52074836368eade8851ea32f1e8ef64e493e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007036"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="7729e-103">tipo de recurso workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7729e-103">workbookWorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7729e-104">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="7729e-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="7729e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7729e-105">Methods</span></span>

| <span data-ttu-id="7729e-106">Método</span><span class="sxs-lookup"><span data-stu-id="7729e-106">Method</span></span>           | <span data-ttu-id="7729e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7729e-107">Return Type</span></span>    |<span data-ttu-id="7729e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7729e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7729e-109">Obter workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7729e-109">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="7729e-110">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7729e-110">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="7729e-111">Leia as propriedades e os relacionamentos do objeto workbookWorksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="7729e-111">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="7729e-112">Protect</span><span class="sxs-lookup"><span data-stu-id="7729e-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="7729e-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7729e-113">None</span></span>|<span data-ttu-id="7729e-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="7729e-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="7729e-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="7729e-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="7729e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7729e-117">None</span></span>|<span data-ttu-id="7729e-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="7729e-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="7729e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7729e-119">Properties</span></span>
| <span data-ttu-id="7729e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7729e-120">Property</span></span>     | <span data-ttu-id="7729e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7729e-121">Type</span></span>   |<span data-ttu-id="7729e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7729e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7729e-123">options</span><span class="sxs-lookup"><span data-stu-id="7729e-123">options</span></span>|[<span data-ttu-id="7729e-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="7729e-124">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="7729e-125">Opções de proteção da planilha.</span><span class="sxs-lookup"><span data-stu-id="7729e-125">Sheet protection options.</span></span> <span data-ttu-id="7729e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7729e-126">Read-only.</span></span>|
|<span data-ttu-id="7729e-127">protected</span><span class="sxs-lookup"><span data-stu-id="7729e-127">protected</span></span>|<span data-ttu-id="7729e-128">booliano</span><span class="sxs-lookup"><span data-stu-id="7729e-128">boolean</span></span>|<span data-ttu-id="7729e-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7729e-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7729e-131">Relações</span><span class="sxs-lookup"><span data-stu-id="7729e-131">Relationships</span></span>
<span data-ttu-id="7729e-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7729e-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7729e-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7729e-133">JSON representation</span></span>

<span data-ttu-id="7729e-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7729e-134">Here is a JSON representation of the resource.</span></span>

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
