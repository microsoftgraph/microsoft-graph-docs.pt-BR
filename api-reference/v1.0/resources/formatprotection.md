---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto range.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: babd1192e216179c59b40d78175f24b0e8366d71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032435"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="5bb3a-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5bb3a-103">FormatProtection resource type</span></span>

<span data-ttu-id="5bb3a-104">Representa a proteção de formatação de um objeto range.</span><span class="sxs-lookup"><span data-stu-id="5bb3a-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="5bb3a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5bb3a-105">Methods</span></span>

| <span data-ttu-id="5bb3a-106">Método</span><span class="sxs-lookup"><span data-stu-id="5bb3a-106">Method</span></span>           | <span data-ttu-id="5bb3a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5bb3a-107">Return Type</span></span>    |<span data-ttu-id="5bb3a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb3a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5bb3a-109">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5bb3a-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="5bb3a-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5bb3a-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="5bb3a-111">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="5bb3a-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="5bb3a-112">Update</span><span class="sxs-lookup"><span data-stu-id="5bb3a-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="5bb3a-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5bb3a-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="5bb3a-114">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="5bb3a-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5bb3a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bb3a-115">Properties</span></span>
| <span data-ttu-id="5bb3a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb3a-116">Property</span></span>     | <span data-ttu-id="5bb3a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb3a-117">Type</span></span>   |<span data-ttu-id="5bb3a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb3a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bb3a-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="5bb3a-119">formulaHidden</span></span>|<span data-ttu-id="5bb3a-120">booliano</span><span class="sxs-lookup"><span data-stu-id="5bb3a-120">boolean</span></span>|<span data-ttu-id="5bb3a-p101">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="5bb3a-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="5bb3a-123">locked</span><span class="sxs-lookup"><span data-stu-id="5bb3a-123">locked</span></span>|<span data-ttu-id="5bb3a-124">booliano</span><span class="sxs-lookup"><span data-stu-id="5bb3a-124">boolean</span></span>|<span data-ttu-id="5bb3a-p102">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="5bb3a-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bb3a-127">Relações</span><span class="sxs-lookup"><span data-stu-id="5bb3a-127">Relationships</span></span>
<span data-ttu-id="5bb3a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5bb3a-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5bb3a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5bb3a-129">JSON representation</span></span>

<span data-ttu-id="5bb3a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5bb3a-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
