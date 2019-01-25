---
title: tipo de recurso de convertIdResult
description: O resultado de uma conversão de formato de ID realizada pela função translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516522"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="3e5b3-103">tipo de recurso de convertIdResult</span><span class="sxs-lookup"><span data-stu-id="3e5b3-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e5b3-104">O resultado de uma conversão de formato de ID realizada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="3e5b3-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="3e5b3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e5b3-105">Properties</span></span>

| <span data-ttu-id="3e5b3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e5b3-106">Property</span></span> | <span data-ttu-id="3e5b3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e5b3-107">Type</span></span> | <span data-ttu-id="3e5b3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e5b3-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="3e5b3-109">SourceId</span><span class="sxs-lookup"><span data-stu-id="3e5b3-109">sourceId</span></span> | <span data-ttu-id="3e5b3-110">String</span><span class="sxs-lookup"><span data-stu-id="3e5b3-110">String</span></span> | <span data-ttu-id="3e5b3-111">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-111">The identifier that was converted.</span></span> <span data-ttu-id="3e5b3-112">Esse valor é o identificador original, não convertido.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="3e5b3-113">Alvo</span><span class="sxs-lookup"><span data-stu-id="3e5b3-113">targetId</span></span> | <span data-ttu-id="3e5b3-114">String</span><span class="sxs-lookup"><span data-stu-id="3e5b3-114">String</span></span> | <span data-ttu-id="3e5b3-115">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-115">The converted identifier.</span></span> <span data-ttu-id="3e5b3-116">Este valor não estiver presente, se a conversão falhou.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="3e5b3-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="3e5b3-117">errorDetails</span></span> | [<span data-ttu-id="3e5b3-118">Erro genérico</span><span class="sxs-lookup"><span data-stu-id="3e5b3-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="3e5b3-119">Um objeto de erro que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="3e5b3-120">Este valor não estiver presente, se a conversão foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e5b3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e5b3-121">JSON representation</span></span>

<span data-ttu-id="3e5b3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e5b3-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
