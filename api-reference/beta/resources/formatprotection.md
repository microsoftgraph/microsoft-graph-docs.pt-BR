---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto range.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 036c09c1d5e4dfec043e6a1dc612aa728d6588f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973538"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="180f8-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="180f8-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="180f8-104">Representa a proteção de formatação de um objeto range.</span><span class="sxs-lookup"><span data-stu-id="180f8-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="180f8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="180f8-105">Methods</span></span>

| <span data-ttu-id="180f8-106">Método</span><span class="sxs-lookup"><span data-stu-id="180f8-106">Method</span></span>           | <span data-ttu-id="180f8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="180f8-107">Return Type</span></span>    |<span data-ttu-id="180f8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="180f8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="180f8-109">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="180f8-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="180f8-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="180f8-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="180f8-111">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="180f8-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="180f8-112">Update</span><span class="sxs-lookup"><span data-stu-id="180f8-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="180f8-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="180f8-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="180f8-114">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="180f8-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="180f8-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="180f8-115">Properties</span></span>
| <span data-ttu-id="180f8-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="180f8-116">Property</span></span>     | <span data-ttu-id="180f8-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="180f8-117">Type</span></span>   |<span data-ttu-id="180f8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="180f8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="180f8-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="180f8-119">formulaHidden</span></span>|<span data-ttu-id="180f8-120">booliano</span><span class="sxs-lookup"><span data-stu-id="180f8-120">boolean</span></span>|<span data-ttu-id="180f8-p101">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="180f8-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="180f8-123">locked</span><span class="sxs-lookup"><span data-stu-id="180f8-123">locked</span></span>|<span data-ttu-id="180f8-124">booliano</span><span class="sxs-lookup"><span data-stu-id="180f8-124">boolean</span></span>|<span data-ttu-id="180f8-p102">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="180f8-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="180f8-127">Relações</span><span class="sxs-lookup"><span data-stu-id="180f8-127">Relationships</span></span>
<span data-ttu-id="180f8-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="180f8-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="180f8-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="180f8-129">JSON representation</span></span>

<span data-ttu-id="180f8-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="180f8-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
