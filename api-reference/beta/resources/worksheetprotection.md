---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6f32ad7b1cc25d9a937f2de68f1bd930d92ec8f9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572931"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="87a57-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="87a57-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87a57-104">Representa a proteção de um objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="87a57-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="87a57-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="87a57-105">Methods</span></span>

| <span data-ttu-id="87a57-106">Método</span><span class="sxs-lookup"><span data-stu-id="87a57-106">Method</span></span>           | <span data-ttu-id="87a57-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87a57-107">Return Type</span></span>    |<span data-ttu-id="87a57-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a57-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="87a57-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="87a57-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="87a57-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="87a57-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="87a57-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="87a57-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="87a57-112">Protect</span><span class="sxs-lookup"><span data-stu-id="87a57-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="87a57-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87a57-113">None</span></span>|<span data-ttu-id="87a57-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="87a57-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="87a57-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="87a57-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="87a57-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87a57-117">None</span></span>|<span data-ttu-id="87a57-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="87a57-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="87a57-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87a57-119">Properties</span></span>
| <span data-ttu-id="87a57-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87a57-120">Property</span></span>     | <span data-ttu-id="87a57-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a57-121">Type</span></span>   |<span data-ttu-id="87a57-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a57-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87a57-123">protected</span><span class="sxs-lookup"><span data-stu-id="87a57-123">protected</span></span>|<span data-ttu-id="87a57-124">booliano</span><span class="sxs-lookup"><span data-stu-id="87a57-124">boolean</span></span>|<span data-ttu-id="87a57-p102">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87a57-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87a57-127">Relações</span><span class="sxs-lookup"><span data-stu-id="87a57-127">Relationships</span></span>
| <span data-ttu-id="87a57-128">Relação</span><span class="sxs-lookup"><span data-stu-id="87a57-128">Relationship</span></span> | <span data-ttu-id="87a57-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a57-129">Type</span></span>   |<span data-ttu-id="87a57-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a57-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87a57-131">options</span><span class="sxs-lookup"><span data-stu-id="87a57-131">options</span></span>|[<span data-ttu-id="87a57-132">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="87a57-132">workbookWorksheetProtection</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="87a57-p103">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87a57-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87a57-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87a57-135">JSON representation</span></span>

<span data-ttu-id="87a57-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87a57-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "options"
  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
