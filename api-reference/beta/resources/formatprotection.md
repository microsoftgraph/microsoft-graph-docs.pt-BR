---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto range.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: cbad1af0eea639b73e06d5678a2293d744964975
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809555"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="593b2-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="593b2-103">FormatProtection resource type</span></span>

<span data-ttu-id="593b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="593b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="593b2-105">Representa a proteção de formatação de um objeto range.</span><span class="sxs-lookup"><span data-stu-id="593b2-105">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="593b2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="593b2-106">Methods</span></span>

| <span data-ttu-id="593b2-107">Método</span><span class="sxs-lookup"><span data-stu-id="593b2-107">Method</span></span>           | <span data-ttu-id="593b2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="593b2-108">Return Type</span></span>    |<span data-ttu-id="593b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="593b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="593b2-110">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="593b2-110">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="593b2-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="593b2-111">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="593b2-112">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="593b2-112">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="593b2-113">Update</span><span class="sxs-lookup"><span data-stu-id="593b2-113">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="593b2-114">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="593b2-114">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="593b2-115">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="593b2-115">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="593b2-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="593b2-116">Properties</span></span>
| <span data-ttu-id="593b2-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="593b2-117">Property</span></span>     | <span data-ttu-id="593b2-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="593b2-118">Type</span></span>   |<span data-ttu-id="593b2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="593b2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="593b2-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="593b2-120">formulaHidden</span></span>|<span data-ttu-id="593b2-121">booliano</span><span class="sxs-lookup"><span data-stu-id="593b2-121">boolean</span></span>|<span data-ttu-id="593b2-p101">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="593b2-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="593b2-124">locked</span><span class="sxs-lookup"><span data-stu-id="593b2-124">locked</span></span>|<span data-ttu-id="593b2-125">booliano</span><span class="sxs-lookup"><span data-stu-id="593b2-125">boolean</span></span>|<span data-ttu-id="593b2-p102">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="593b2-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="593b2-128">Relações</span><span class="sxs-lookup"><span data-stu-id="593b2-128">Relationships</span></span>
<span data-ttu-id="593b2-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="593b2-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="593b2-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="593b2-130">JSON representation</span></span>

<span data-ttu-id="593b2-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="593b2-131">Here is a JSON representation of the resource.</span></span>

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
