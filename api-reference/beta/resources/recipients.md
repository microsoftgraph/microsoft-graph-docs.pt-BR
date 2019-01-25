---
title: tipo de recurso de destinatários
description: Veja a seguir uma representação JSON do recurso
localization_priority: Normal
ms.openlocfilehash: 1ba4e8c88de3ba96e5e846cb5be8261562567ac3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507835"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="b16f2-103">tipo de recurso de destinatários</span><span class="sxs-lookup"><span data-stu-id="b16f2-103">recipients resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="b16f2-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b16f2-104">JSON representation</span></span>

<span data-ttu-id="b16f2-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b16f2-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b16f2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b16f2-106">Properties</span></span>
| <span data-ttu-id="b16f2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b16f2-107">Property</span></span>     | <span data-ttu-id="b16f2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b16f2-108">Type</span></span>   |<span data-ttu-id="b16f2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b16f2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b16f2-110">alias</span><span class="sxs-lookup"><span data-stu-id="b16f2-110">alias</span></span>|<span data-ttu-id="b16f2-111">String</span><span class="sxs-lookup"><span data-stu-id="b16f2-111">String</span></span>||
|<span data-ttu-id="b16f2-112">email</span><span class="sxs-lookup"><span data-stu-id="b16f2-112">email</span></span>|<span data-ttu-id="b16f2-113">String</span><span class="sxs-lookup"><span data-stu-id="b16f2-113">String</span></span>||
|<span data-ttu-id="b16f2-114">objectId</span><span class="sxs-lookup"><span data-stu-id="b16f2-114">objectId</span></span>|<span data-ttu-id="b16f2-115">String</span><span class="sxs-lookup"><span data-stu-id="b16f2-115">String</span></span>||
|<span data-ttu-id="b16f2-116">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="b16f2-116">permissionIdentityType</span></span>|<span data-ttu-id="b16f2-117">String</span><span class="sxs-lookup"><span data-stu-id="b16f2-117">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recipients.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
