---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto range.
localization_priority: Normal
ms.openlocfilehash: 7375ea26caef3d8b06421441a712974c209b53ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333680"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="8b74a-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="8b74a-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b74a-104">Representa a proteção de formatação de um objeto range.</span><span class="sxs-lookup"><span data-stu-id="8b74a-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="8b74a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b74a-105">Methods</span></span>

| <span data-ttu-id="8b74a-106">Método</span><span class="sxs-lookup"><span data-stu-id="8b74a-106">Method</span></span>           | <span data-ttu-id="8b74a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b74a-107">Return Type</span></span>    |<span data-ttu-id="8b74a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b74a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b74a-109">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="8b74a-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="8b74a-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="8b74a-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="8b74a-111">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="8b74a-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="8b74a-112">Update</span><span class="sxs-lookup"><span data-stu-id="8b74a-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="8b74a-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="8b74a-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="8b74a-114">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="8b74a-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8b74a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b74a-115">Properties</span></span>
| <span data-ttu-id="8b74a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b74a-116">Property</span></span>     | <span data-ttu-id="8b74a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b74a-117">Type</span></span>   |<span data-ttu-id="8b74a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b74a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b74a-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="8b74a-119">formulaHidden</span></span>|<span data-ttu-id="8b74a-120">booliano</span><span class="sxs-lookup"><span data-stu-id="8b74a-120">boolean</span></span>|<span data-ttu-id="8b74a-p101">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="8b74a-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="8b74a-123">locked</span><span class="sxs-lookup"><span data-stu-id="8b74a-123">locked</span></span>|<span data-ttu-id="8b74a-124">booliano</span><span class="sxs-lookup"><span data-stu-id="8b74a-124">boolean</span></span>|<span data-ttu-id="8b74a-p102">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="8b74a-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b74a-127">Relações</span><span class="sxs-lookup"><span data-stu-id="8b74a-127">Relationships</span></span>
<span data-ttu-id="8b74a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b74a-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b74a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b74a-129">JSON representation</span></span>

<span data-ttu-id="8b74a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b74a-130">Here is a JSON representation of the resource.</span></span>

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
