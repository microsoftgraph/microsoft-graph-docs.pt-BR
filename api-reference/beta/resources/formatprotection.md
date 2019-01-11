---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto de intervalo.
localization_priority: Normal
ms.openlocfilehash: 0b4add2e30a1e475adcb162903f771ce760f9285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805618"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="91bee-103">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="91bee-103">FormatProtection resource type</span></span>

> <span data-ttu-id="91bee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91bee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91bee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91bee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91bee-106">Representa a proteção de formatação de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="91bee-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="91bee-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="91bee-107">Methods</span></span>

| <span data-ttu-id="91bee-108">Método</span><span class="sxs-lookup"><span data-stu-id="91bee-108">Method</span></span>           | <span data-ttu-id="91bee-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="91bee-109">Return Type</span></span>    |<span data-ttu-id="91bee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bee-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91bee-111">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="91bee-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="91bee-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="91bee-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="91bee-113">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="91bee-113">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="91bee-114">Update</span><span class="sxs-lookup"><span data-stu-id="91bee-114">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="91bee-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="91bee-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="91bee-116">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="91bee-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="91bee-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91bee-117">Properties</span></span>
| <span data-ttu-id="91bee-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91bee-118">Property</span></span>     | <span data-ttu-id="91bee-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="91bee-119">Type</span></span>   |<span data-ttu-id="91bee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bee-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91bee-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="91bee-121">formulaHidden</span></span>|<span data-ttu-id="91bee-122">booliano</span><span class="sxs-lookup"><span data-stu-id="91bee-122">boolean</span></span>|<span data-ttu-id="91bee-p102">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="91bee-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="91bee-125">locked</span><span class="sxs-lookup"><span data-stu-id="91bee-125">locked</span></span>|<span data-ttu-id="91bee-126">booliano</span><span class="sxs-lookup"><span data-stu-id="91bee-126">boolean</span></span>|<span data-ttu-id="91bee-p103">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="91bee-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91bee-129">Relações</span><span class="sxs-lookup"><span data-stu-id="91bee-129">Relationships</span></span>
<span data-ttu-id="91bee-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91bee-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="91bee-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91bee-131">JSON representation</span></span>

<span data-ttu-id="91bee-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91bee-132">Here is a JSON representation of the resource.</span></span>

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
