---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29639941"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="3c044-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="3c044-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c044-104">Representa a proteção de um objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="3c044-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="3c044-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c044-105">Methods</span></span>

| <span data-ttu-id="3c044-106">Método</span><span class="sxs-lookup"><span data-stu-id="3c044-106">Method</span></span>           | <span data-ttu-id="3c044-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3c044-107">Return Type</span></span>    |<span data-ttu-id="3c044-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c044-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c044-109">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="3c044-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="3c044-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="3c044-110">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="3c044-111">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="3c044-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="3c044-112">Protect</span><span class="sxs-lookup"><span data-stu-id="3c044-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="3c044-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c044-113">None</span></span>|<span data-ttu-id="3c044-p101">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="3c044-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="3c044-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="3c044-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="3c044-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c044-117">None</span></span>|<span data-ttu-id="3c044-118">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="3c044-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="3c044-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c044-119">Properties</span></span>
| <span data-ttu-id="3c044-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c044-120">Property</span></span>     | <span data-ttu-id="3c044-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c044-121">Type</span></span>   |<span data-ttu-id="3c044-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c044-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c044-123">protected</span><span class="sxs-lookup"><span data-stu-id="3c044-123">protected</span></span>|<span data-ttu-id="3c044-124">booliano</span><span class="sxs-lookup"><span data-stu-id="3c044-124">boolean</span></span>|<span data-ttu-id="3c044-p102">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c044-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c044-127">Relações</span><span class="sxs-lookup"><span data-stu-id="3c044-127">Relationships</span></span>
| <span data-ttu-id="3c044-128">Relação</span><span class="sxs-lookup"><span data-stu-id="3c044-128">Relationship</span></span> | <span data-ttu-id="3c044-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c044-129">Type</span></span>   |<span data-ttu-id="3c044-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c044-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c044-131">options</span><span class="sxs-lookup"><span data-stu-id="3c044-131">options</span></span>|[<span data-ttu-id="3c044-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="3c044-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="3c044-p103">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c044-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c044-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c044-135">JSON representation</span></span>

<span data-ttu-id="3c044-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c044-136">Here is a JSON representation of the resource.</span></span>

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
