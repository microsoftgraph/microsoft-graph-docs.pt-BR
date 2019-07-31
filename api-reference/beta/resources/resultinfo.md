---
title: tipo de recurso resultInfo
description: O tipo resultInfo.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1e5f6a523a8aca4454cd3355e2a0287fef9fc90d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965366"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="50de9-103">tipo de recurso resultInfo</span><span class="sxs-lookup"><span data-stu-id="50de9-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50de9-104">O tipo resultInfo.</span><span class="sxs-lookup"><span data-stu-id="50de9-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="50de9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50de9-105">Properties</span></span>

| <span data-ttu-id="50de9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50de9-106">Property</span></span> | <span data-ttu-id="50de9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="50de9-107">Type</span></span>   | <span data-ttu-id="50de9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="50de9-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="50de9-109">código</span><span class="sxs-lookup"><span data-stu-id="50de9-109">code</span></span>     | <span data-ttu-id="50de9-110">String</span><span class="sxs-lookup"><span data-stu-id="50de9-110">String</span></span> | <span data-ttu-id="50de9-111">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="50de9-111">The result code.</span></span>     |
| <span data-ttu-id="50de9-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="50de9-112">message</span></span>  | <span data-ttu-id="50de9-113">String</span><span class="sxs-lookup"><span data-stu-id="50de9-113">String</span></span> | <span data-ttu-id="50de9-114">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="50de9-114">The message.</span></span>         |
| <span data-ttu-id="50de9-115">Subcódigo</span><span class="sxs-lookup"><span data-stu-id="50de9-115">subCode</span></span>  | <span data-ttu-id="50de9-116">String</span><span class="sxs-lookup"><span data-stu-id="50de9-116">String</span></span> | <span data-ttu-id="50de9-117">O subcódigo do resultado.</span><span class="sxs-lookup"><span data-stu-id="50de9-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50de9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50de9-118">JSON representation</span></span>

<span data-ttu-id="50de9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50de9-119">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="50de9-120">Exemplo de resultado de erro</span><span class="sxs-lookup"><span data-stu-id="50de9-120">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="50de9-121">Exemplo de resultado genérico de êxito</span><span class="sxs-lookup"><span data-stu-id="50de9-121">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="50de9-122">Resultado de êxito do registro de exemplo</span><span class="sxs-lookup"><span data-stu-id="50de9-122">Example Record Success result</span></span>

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
  "suppressions": []
}
-->
