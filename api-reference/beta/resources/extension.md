---
title: Tipo de recurso extension
description: Um tipo abstrato para oferecer suporte ao tipo openTypeExtension livre do OData v4.
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512742"
---
# <a name="extension-resource-type"></a><span data-ttu-id="9fa3c-103">Tipo de recurso extension</span><span class="sxs-lookup"><span data-stu-id="9fa3c-103">extension resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fa3c-104">Um tipo abstrato para oferecer suporte ao tipo [openTypeExtension](opentypeextension.md) livre do OData v4.</span><span class="sxs-lookup"><span data-stu-id="9fa3c-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fa3c-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fa3c-105">JSON representation</span></span>

<span data-ttu-id="9fa3c-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9fa3c-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="9fa3c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fa3c-107">Properties</span></span>
| <span data-ttu-id="9fa3c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fa3c-108">Property</span></span>     | <span data-ttu-id="9fa3c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fa3c-109">Type</span></span>   |<span data-ttu-id="9fa3c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fa3c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fa3c-111">id</span><span class="sxs-lookup"><span data-stu-id="9fa3c-111">id</span></span>|<span data-ttu-id="9fa3c-112">String</span><span class="sxs-lookup"><span data-stu-id="9fa3c-112">String</span></span>| <span data-ttu-id="9fa3c-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fa3c-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa3c-114">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="9fa3c-114">Relationships</span></span>
<span data-ttu-id="9fa3c-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fa3c-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="9fa3c-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="9fa3c-116">Methods</span></span>

<span data-ttu-id="9fa3c-117">Consulte os métodos do tipo derivado [openTypeExtension](opentypeextension.md) para métodos que são realmente compatíveis.</span><span class="sxs-lookup"><span data-stu-id="9fa3c-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
