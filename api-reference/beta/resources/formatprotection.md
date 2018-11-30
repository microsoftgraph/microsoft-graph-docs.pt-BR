---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto de intervalo.
ms.openlocfilehash: 5f2a4968b018a952b24bb18a75a4f6d5aff55b00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037741"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="d60b3-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d60b3-103">FormatProtection resource type</span></span>

> <span data-ttu-id="d60b3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d60b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d60b3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d60b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d60b3-106">Representa a proteção de formatação de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="d60b3-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="d60b3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d60b3-107">Methods</span></span>

| <span data-ttu-id="d60b3-108">Método</span><span class="sxs-lookup"><span data-stu-id="d60b3-108">Method</span></span>           | <span data-ttu-id="d60b3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d60b3-109">Return Type</span></span>    |<span data-ttu-id="d60b3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d60b3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d60b3-111">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d60b3-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="d60b3-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d60b3-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="d60b3-113">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="d60b3-113">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="d60b3-114">Update</span><span class="sxs-lookup"><span data-stu-id="d60b3-114">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="d60b3-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d60b3-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="d60b3-116">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="d60b3-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d60b3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d60b3-117">Properties</span></span>
| <span data-ttu-id="d60b3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d60b3-118">Property</span></span>     | <span data-ttu-id="d60b3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d60b3-119">Type</span></span>   |<span data-ttu-id="d60b3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d60b3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d60b3-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="d60b3-121">formulaHidden</span></span>|<span data-ttu-id="d60b3-122">booliano</span><span class="sxs-lookup"><span data-stu-id="d60b3-122">boolean</span></span>|<span data-ttu-id="d60b3-p102">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="d60b3-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="d60b3-125">locked</span><span class="sxs-lookup"><span data-stu-id="d60b3-125">locked</span></span>|<span data-ttu-id="d60b3-126">booliano</span><span class="sxs-lookup"><span data-stu-id="d60b3-126">boolean</span></span>|<span data-ttu-id="d60b3-p103">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="d60b3-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d60b3-129">Relações</span><span class="sxs-lookup"><span data-stu-id="d60b3-129">Relationships</span></span>
<span data-ttu-id="d60b3-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d60b3-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d60b3-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d60b3-131">JSON representation</span></span>

<span data-ttu-id="d60b3-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d60b3-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->