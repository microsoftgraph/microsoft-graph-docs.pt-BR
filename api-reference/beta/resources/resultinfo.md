---
title: tipo de recurso de resultInfo
description: O tipo de resultInfo.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521079"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="0b6b0-103">tipo de recurso de resultInfo</span><span class="sxs-lookup"><span data-stu-id="0b6b0-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b6b0-104">O tipo de resultInfo.</span><span class="sxs-lookup"><span data-stu-id="0b6b0-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="0b6b0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b6b0-105">Properties</span></span>

| <span data-ttu-id="0b6b0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b6b0-106">Property</span></span> | <span data-ttu-id="0b6b0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b6b0-107">Type</span></span>   | <span data-ttu-id="0b6b0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b6b0-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="0b6b0-109">código</span><span class="sxs-lookup"><span data-stu-id="0b6b0-109">code</span></span>     | <span data-ttu-id="0b6b0-110">String</span><span class="sxs-lookup"><span data-stu-id="0b6b0-110">String</span></span> | <span data-ttu-id="0b6b0-111">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="0b6b0-111">The result code.</span></span>     |
| <span data-ttu-id="0b6b0-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="0b6b0-112">message</span></span>  | <span data-ttu-id="0b6b0-113">String</span><span class="sxs-lookup"><span data-stu-id="0b6b0-113">String</span></span> | <span data-ttu-id="0b6b0-114">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="0b6b0-114">The message.</span></span>         |
| <span data-ttu-id="0b6b0-115">Subcódigo</span><span class="sxs-lookup"><span data-stu-id="0b6b0-115">subCode</span></span>  | <span data-ttu-id="0b6b0-116">String</span><span class="sxs-lookup"><span data-stu-id="0b6b0-116">String</span></span> | <span data-ttu-id="0b6b0-117">O código de resultado de subsites.</span><span class="sxs-lookup"><span data-stu-id="0b6b0-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b6b0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b6b0-118">JSON representation</span></span>

<span data-ttu-id="0b6b0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b6b0-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="0b6b0-120">Resultado de erro de exemplo</span><span class="sxs-lookup"><span data-stu-id="0b6b0-120">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="0b6b0-121">Resultado de sucesso genérico de exemplo</span><span class="sxs-lookup"><span data-stu-id="0b6b0-121">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="0b6b0-122">Resultado de sucesso do registro de exemplo</span><span class="sxs-lookup"><span data-stu-id="0b6b0-122">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resultinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
