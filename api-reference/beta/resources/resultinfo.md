---
title: tipo de recurso de resultInfo
description: O tipo de resultInfo.
ms.openlocfilehash: 93dc08407608a87cbc1cfa027f5c8f20483834e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035229"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="90809-103">tipo de recurso de resultInfo</span><span class="sxs-lookup"><span data-stu-id="90809-103">resultInfo resource type</span></span>

> <span data-ttu-id="90809-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90809-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90809-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90809-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90809-106">O tipo de resultInfo.</span><span class="sxs-lookup"><span data-stu-id="90809-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="90809-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90809-107">Properties</span></span>

| <span data-ttu-id="90809-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90809-108">Property</span></span> | <span data-ttu-id="90809-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="90809-109">Type</span></span>   | <span data-ttu-id="90809-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="90809-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="90809-111">código</span><span class="sxs-lookup"><span data-stu-id="90809-111">code</span></span>     | <span data-ttu-id="90809-112">String</span><span class="sxs-lookup"><span data-stu-id="90809-112">String</span></span> | <span data-ttu-id="90809-113">O código de resultado.</span><span class="sxs-lookup"><span data-stu-id="90809-113">The result code.</span></span>     |
| <span data-ttu-id="90809-114">mensagem</span><span class="sxs-lookup"><span data-stu-id="90809-114">message</span></span>  | <span data-ttu-id="90809-115">String</span><span class="sxs-lookup"><span data-stu-id="90809-115">String</span></span> | <span data-ttu-id="90809-116">A mensagem.</span><span class="sxs-lookup"><span data-stu-id="90809-116">The message.</span></span>         |
| <span data-ttu-id="90809-117">Subcódigo</span><span class="sxs-lookup"><span data-stu-id="90809-117">subCode</span></span>  | <span data-ttu-id="90809-118">String</span><span class="sxs-lookup"><span data-stu-id="90809-118">String</span></span> | <span data-ttu-id="90809-119">O código de resultado de subsites.</span><span class="sxs-lookup"><span data-stu-id="90809-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="90809-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90809-120">JSON representation</span></span>

<span data-ttu-id="90809-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90809-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="90809-122">Resultado de erro de exemplo</span><span class="sxs-lookup"><span data-stu-id="90809-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="90809-123">Resultado de sucesso genérico de exemplo</span><span class="sxs-lookup"><span data-stu-id="90809-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="90809-124">Resultado de sucesso do registro de exemplo</span><span class="sxs-lookup"><span data-stu-id="90809-124">Example Record Success result</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
