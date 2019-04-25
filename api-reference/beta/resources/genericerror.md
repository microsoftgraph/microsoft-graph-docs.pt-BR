---
title: tipo de recurso genericError
description: Um erro de uso geral.
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547491"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="23f0e-103">tipo de recurso genericError</span><span class="sxs-lookup"><span data-stu-id="23f0e-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f0e-104">Um erro de uso geral.</span><span class="sxs-lookup"><span data-stu-id="23f0e-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="23f0e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23f0e-105">Properties</span></span>

| <span data-ttu-id="23f0e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23f0e-106">Property</span></span> | <span data-ttu-id="23f0e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="23f0e-107">Type</span></span> | <span data-ttu-id="23f0e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f0e-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="23f0e-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="23f0e-109">message</span></span> | <span data-ttu-id="23f0e-110">String</span><span class="sxs-lookup"><span data-stu-id="23f0e-110">String</span></span> | <span data-ttu-id="23f0e-111">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="23f0e-111">The error message.</span></span> |
| <span data-ttu-id="23f0e-112">código</span><span class="sxs-lookup"><span data-stu-id="23f0e-112">code</span></span> | <span data-ttu-id="23f0e-113">String</span><span class="sxs-lookup"><span data-stu-id="23f0e-113">String</span></span> | <span data-ttu-id="23f0e-114">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="23f0e-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="23f0e-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23f0e-115">JSON representation</span></span>

<span data-ttu-id="23f0e-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23f0e-116">Here is a JSON representation of the resource.</span></span>

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
