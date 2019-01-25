---
title: tipo de recurso de mailTipsError
description: Um erro que ocorre durante uma ação.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e8a029eb00e5419f8c0e945e71dd0ba1ed2e147
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523985"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="bcb4b-103">tipo de recurso de mailTipsError</span><span class="sxs-lookup"><span data-stu-id="bcb4b-103">mailTipsError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcb4b-104">Um erro que ocorre durante uma ação.</span><span class="sxs-lookup"><span data-stu-id="bcb4b-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="bcb4b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcb4b-105">Properties</span></span>
| <span data-ttu-id="bcb4b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcb4b-106">Property</span></span>     | <span data-ttu-id="bcb4b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcb4b-107">Type</span></span>   |<span data-ttu-id="bcb4b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcb4b-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="bcb4b-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="bcb4b-109">message</span></span> | <span data-ttu-id="bcb4b-110">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-110">String</span></span> | <span data-ttu-id="bcb4b-111">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="bcb4b-111">The error message.</span></span> |
| <span data-ttu-id="bcb4b-112">código</span><span class="sxs-lookup"><span data-stu-id="bcb4b-112">code</span></span> | <span data-ttu-id="bcb4b-113">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-113">String</span></span> | <span data-ttu-id="bcb4b-114">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="bcb4b-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bcb4b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcb4b-115">JSON representation</span></span>

<span data-ttu-id="bcb4b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcb4b-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtipserror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
