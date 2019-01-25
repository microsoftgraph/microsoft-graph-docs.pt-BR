---
title: tipo de recurso de erro genérico
description: Um erro de finalidade geral.
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524125"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="ce94a-103">tipo de recurso de erro genérico</span><span class="sxs-lookup"><span data-stu-id="ce94a-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce94a-104">Um erro de finalidade geral.</span><span class="sxs-lookup"><span data-stu-id="ce94a-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="ce94a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce94a-105">Properties</span></span>

| <span data-ttu-id="ce94a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce94a-106">Property</span></span> | <span data-ttu-id="ce94a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce94a-107">Type</span></span> | <span data-ttu-id="ce94a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce94a-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ce94a-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="ce94a-109">message</span></span> | <span data-ttu-id="ce94a-110">String</span><span class="sxs-lookup"><span data-stu-id="ce94a-110">String</span></span> | <span data-ttu-id="ce94a-111">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="ce94a-111">The error message.</span></span> |
| <span data-ttu-id="ce94a-112">código</span><span class="sxs-lookup"><span data-stu-id="ce94a-112">code</span></span> | <span data-ttu-id="ce94a-113">String</span><span class="sxs-lookup"><span data-stu-id="ce94a-113">String</span></span> | <span data-ttu-id="ce94a-114">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="ce94a-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce94a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce94a-115">JSON representation</span></span>

<span data-ttu-id="ce94a-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce94a-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
