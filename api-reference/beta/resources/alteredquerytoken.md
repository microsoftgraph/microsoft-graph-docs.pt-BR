---
title: Tipo de recurso alteredQueryToken
description: Representa segmentos alterados em relação à consulta de usuário original.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 03e6f010fdcd77e07fc6ce3cc7e8c8c285fde73f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067834"
---
# <a name="alteredquerytoken-resource-type"></a><span data-ttu-id="b0b21-103">Tipo de recurso alteredQueryToken</span><span class="sxs-lookup"><span data-stu-id="b0b21-103">alteredQueryToken resource type</span></span>

<span data-ttu-id="b0b21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0b21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0b21-105">Representa segmentos alterados em relação à consulta de usuário original.</span><span class="sxs-lookup"><span data-stu-id="b0b21-105">Represents changed segments with respect to original user query.</span></span>

## <a name="properties"></a><span data-ttu-id="b0b21-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0b21-106">Properties</span></span>

| <span data-ttu-id="b0b21-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0b21-107">Property</span></span>     | <span data-ttu-id="b0b21-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0b21-108">Type</span></span>        | <span data-ttu-id="b0b21-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0b21-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0b21-110">offset</span><span class="sxs-lookup"><span data-stu-id="b0b21-110">offset</span></span>|<span data-ttu-id="b0b21-111">Int32</span><span class="sxs-lookup"><span data-stu-id="b0b21-111">Int32</span></span>| <span data-ttu-id="b0b21-112">Define o deslocamento de um segmento alterado.</span><span class="sxs-lookup"><span data-stu-id="b0b21-112">Defines the offset of a changed segment.</span></span>|
|<span data-ttu-id="b0b21-113">length</span><span class="sxs-lookup"><span data-stu-id="b0b21-113">length</span></span>|<span data-ttu-id="b0b21-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b0b21-114">Int32</span></span>| <span data-ttu-id="b0b21-115">Define o comprimento de um segmento alterado.</span><span class="sxs-lookup"><span data-stu-id="b0b21-115">Defines the length of a changed segment.</span></span>|
|<span data-ttu-id="b0b21-116">suggestion</span><span class="sxs-lookup"><span data-stu-id="b0b21-116">suggestion</span></span>|<span data-ttu-id="b0b21-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0b21-117">String</span></span>| <span data-ttu-id="b0b21-118">Representa a cadeia de caracteres de segmento corrigido.</span><span class="sxs-lookup"><span data-stu-id="b0b21-118">Represents the corrected segment string.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0b21-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0b21-119">JSON representation</span></span>

<span data-ttu-id="b0b21-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0b21-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "offset": 0,
  "length": 6,
  "suggestion": "String"
}
```
