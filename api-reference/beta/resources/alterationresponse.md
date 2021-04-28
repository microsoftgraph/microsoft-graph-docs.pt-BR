---
title: Tipo de recurso de alterationResponse
description: Fornece informações relacionadas a correções ortográficas na resposta à alteração.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e23b94b4e35776b2278c7818efc71f14edcc6cbb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067883"
---
# <a name="alterationresponse-resource-type"></a><span data-ttu-id="50f07-103">Tipo de recurso de alterationResponse</span><span class="sxs-lookup"><span data-stu-id="50f07-103">alterationResponse resource type</span></span>

<span data-ttu-id="50f07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50f07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50f07-105">Fornece informações relacionadas a correções ortográficas na resposta à alteração.</span><span class="sxs-lookup"><span data-stu-id="50f07-105">Provides information related to spelling corrections in the alteration response.</span></span>

## <a name="properties"></a><span data-ttu-id="50f07-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50f07-106">Properties</span></span>

| <span data-ttu-id="50f07-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50f07-107">Property</span></span>     | <span data-ttu-id="50f07-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="50f07-108">Type</span></span>        | <span data-ttu-id="50f07-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f07-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50f07-110">originalQueryString</span><span class="sxs-lookup"><span data-stu-id="50f07-110">originalQueryString</span></span>|<span data-ttu-id="50f07-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50f07-111">String</span></span>| <span data-ttu-id="50f07-112">Define a cadeia de caracteres de consulta do usuário original.</span><span class="sxs-lookup"><span data-stu-id="50f07-112">Defines the original user query string.</span></span>|
|<span data-ttu-id="50f07-113">queryAlteration</span><span class="sxs-lookup"><span data-stu-id="50f07-113">queryAlteration</span></span>|[<span data-ttu-id="50f07-114">searchAlteration</span><span class="sxs-lookup"><span data-stu-id="50f07-114">searchAlteration</span></span>](searchalteration.md)| <span data-ttu-id="50f07-115">Define os detalhes das informações de alteração para a correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="50f07-115">Defines the details of alteration information for the spelling correction.</span></span>|
|<span data-ttu-id="50f07-116">queryAlterationType</span><span class="sxs-lookup"><span data-stu-id="50f07-116">queryAlterationType</span></span>|<span data-ttu-id="50f07-117">searchAlterationType</span><span class="sxs-lookup"><span data-stu-id="50f07-117">searchAlterationType</span></span>| <span data-ttu-id="50f07-118">Define o tipo de correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="50f07-118">Defines the type of the spelling correction.</span></span> <span data-ttu-id="50f07-119">Os valores possíveis `suggestion` são , `modification` .</span><span class="sxs-lookup"><span data-stu-id="50f07-119">Possible values are `suggestion`, `modification`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50f07-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50f07-120">JSON representation</span></span>

<span data-ttu-id="50f07-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50f07-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "suggestion"
}
```
