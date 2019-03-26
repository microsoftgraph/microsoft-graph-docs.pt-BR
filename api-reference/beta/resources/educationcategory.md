---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800946"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="57eb9-103">tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="57eb9-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57eb9-104">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="57eb9-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="57eb9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="57eb9-105">Methods</span></span>

| <span data-ttu-id="57eb9-106">Método</span><span class="sxs-lookup"><span data-stu-id="57eb9-106">Method</span></span>           | <span data-ttu-id="57eb9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57eb9-107">Return Type</span></span>    |<span data-ttu-id="57eb9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="57eb9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="57eb9-109">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="57eb9-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="57eb9-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="57eb9-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="57eb9-111">Obter um **educationCategory**existente.</span><span class="sxs-lookup"><span data-stu-id="57eb9-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="57eb9-112">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="57eb9-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="57eb9-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57eb9-113">None</span></span> | <span data-ttu-id="57eb9-114">Remover um **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="57eb9-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="57eb9-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57eb9-115">Properties</span></span>
| <span data-ttu-id="57eb9-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57eb9-116">Property</span></span>     | <span data-ttu-id="57eb9-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="57eb9-117">Type</span></span>   |<span data-ttu-id="57eb9-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="57eb9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57eb9-119">id</span><span class="sxs-lookup"><span data-stu-id="57eb9-119">id</span></span>|<span data-ttu-id="57eb9-120">String</span><span class="sxs-lookup"><span data-stu-id="57eb9-120">String</span></span>|<span data-ttu-id="57eb9-121">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="57eb9-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="57eb9-122">displayName</span><span class="sxs-lookup"><span data-stu-id="57eb9-122">displayName</span></span>|<span data-ttu-id="57eb9-123">String</span><span class="sxs-lookup"><span data-stu-id="57eb9-123">String</span></span>|<span data-ttu-id="57eb9-124">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="57eb9-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57eb9-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57eb9-125">JSON representation</span></span>

<span data-ttu-id="57eb9-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57eb9-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
