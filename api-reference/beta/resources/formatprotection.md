---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto de intervalo.
localization_priority: Normal
ms.openlocfilehash: 7bc27060567136386ef1f08e6fe46e95980788a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509186"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="1e616-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="1e616-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e616-104">Representa a proteção de formatação de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="1e616-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="1e616-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1e616-105">Methods</span></span>

| <span data-ttu-id="1e616-106">Método</span><span class="sxs-lookup"><span data-stu-id="1e616-106">Method</span></span>           | <span data-ttu-id="1e616-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1e616-107">Return Type</span></span>    |<span data-ttu-id="1e616-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e616-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e616-109">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="1e616-109">[Get FormatProtection](../api/formatprotection-get.md)</span></span> | [<span data-ttu-id="1e616-110">formatProtection</span><span class="sxs-lookup"><span data-stu-id="1e616-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="1e616-111">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="1e616-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="1e616-112">Update</span><span class="sxs-lookup"><span data-stu-id="1e616-112">Update</span></span>](../api/formatprotection-update.md) | <span data-ttu-id="1e616-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="1e616-113">[FormatProtection](formatprotection.md)</span></span>  |<span data-ttu-id="1e616-114">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="1e616-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e616-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e616-115">Properties</span></span>
| <span data-ttu-id="1e616-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e616-116">Property</span></span>     | <span data-ttu-id="1e616-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e616-117">Type</span></span>   |<span data-ttu-id="1e616-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e616-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e616-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="1e616-119">formulaHidden</span></span>|<span data-ttu-id="1e616-120">booliano</span><span class="sxs-lookup"><span data-stu-id="1e616-120">boolean</span></span>|<span data-ttu-id="1e616-p101">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="1e616-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="1e616-123">locked</span><span class="sxs-lookup"><span data-stu-id="1e616-123">locked</span></span>|<span data-ttu-id="1e616-124">booliano</span><span class="sxs-lookup"><span data-stu-id="1e616-124">boolean</span></span>|<span data-ttu-id="1e616-p102">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="1e616-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e616-127">Relações</span><span class="sxs-lookup"><span data-stu-id="1e616-127">Relationships</span></span>
<span data-ttu-id="1e616-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e616-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e616-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e616-129">JSON representation</span></span>

<span data-ttu-id="1e616-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e616-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/formatprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
