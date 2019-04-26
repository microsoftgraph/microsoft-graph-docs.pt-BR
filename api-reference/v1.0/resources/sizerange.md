---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
ms.openlocfilehash: ae754d0666185023272860864ef17f038aecff7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552746"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="42d73-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="42d73-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d73-104">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="42d73-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="42d73-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42d73-105">Properties</span></span>
| <span data-ttu-id="42d73-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42d73-106">Property</span></span>     | <span data-ttu-id="42d73-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d73-107">Type</span></span>   |<span data-ttu-id="42d73-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d73-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42d73-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="42d73-109">maximumSize</span></span> | <span data-ttu-id="42d73-110">Int32</span><span class="sxs-lookup"><span data-stu-id="42d73-110">Int32</span></span> | <span data-ttu-id="42d73-111">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="42d73-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="42d73-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="42d73-112">minimumSize</span></span> | <span data-ttu-id="42d73-113">Int32</span><span class="sxs-lookup"><span data-stu-id="42d73-113">Int32</span></span> | <span data-ttu-id="42d73-114">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="42d73-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="42d73-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42d73-115">JSON representation</span></span>
<span data-ttu-id="42d73-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42d73-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sizerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
