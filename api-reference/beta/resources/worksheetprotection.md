---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto sheet.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523799"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="d9b2a-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d9b2a-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9b2a-104">Representa a proteção de um objeto sheet.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="d9b2a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9b2a-105">Methods</span></span>

| <span data-ttu-id="d9b2a-106">Método</span><span class="sxs-lookup"><span data-stu-id="d9b2a-106">Method</span></span>           | <span data-ttu-id="d9b2a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d9b2a-107">Return Type</span></span>    |<span data-ttu-id="d9b2a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b2a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9b2a-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d9b2a-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="d9b2a-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d9b2a-110">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="d9b2a-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="d9b2a-112">Protect</span><span class="sxs-lookup"><span data-stu-id="d9b2a-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="d9b2a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9b2a-113">None</span></span>|<span data-ttu-id="d9b2a-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="d9b2a-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="d9b2a-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="d9b2a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9b2a-117">None</span></span>|<span data-ttu-id="d9b2a-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="d9b2a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9b2a-119">Properties</span></span>
| <span data-ttu-id="d9b2a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9b2a-120">Property</span></span>     | <span data-ttu-id="d9b2a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b2a-121">Type</span></span>   |<span data-ttu-id="d9b2a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b2a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9b2a-123">protected</span><span class="sxs-lookup"><span data-stu-id="d9b2a-123">protected</span></span>|<span data-ttu-id="d9b2a-124">booliano</span><span class="sxs-lookup"><span data-stu-id="d9b2a-124">boolean</span></span>|<span data-ttu-id="d9b2a-p102">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9b2a-127">Relações</span><span class="sxs-lookup"><span data-stu-id="d9b2a-127">Relationships</span></span>
| <span data-ttu-id="d9b2a-128">Relação</span><span class="sxs-lookup"><span data-stu-id="d9b2a-128">Relationship</span></span> | <span data-ttu-id="d9b2a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b2a-129">Type</span></span>   |<span data-ttu-id="d9b2a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b2a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9b2a-131">options</span><span class="sxs-lookup"><span data-stu-id="d9b2a-131">options</span></span>|[<span data-ttu-id="d9b2a-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d9b2a-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="d9b2a-p103">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9b2a-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9b2a-135">JSON representation</span></span>

<span data-ttu-id="d9b2a-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9b2a-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
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
