---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 123d57b05950203434ac23fd85e9c29dfa41476d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067093"
---
# <a name="search-resource-type"></a><span data-ttu-id="acfd3-103">tipo de recurso de pesquisa</span><span class="sxs-lookup"><span data-stu-id="acfd3-103">search resource type</span></span>

<span data-ttu-id="acfd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acfd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acfd3-105">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="acfd3-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="acfd3-106">Ele serve como uma âncora para a [ação de](../api/search-query.md) consulta.</span><span class="sxs-lookup"><span data-stu-id="acfd3-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="acfd3-107">Não é esperado que esse recurso seja chamado dessa forma.</span><span class="sxs-lookup"><span data-stu-id="acfd3-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="acfd3-108">Qualquer solicitação no recurso incorre em uma Solicitação Inovada.</span><span class="sxs-lookup"><span data-stu-id="acfd3-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="acfd3-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acfd3-109">JSON representation</span></span>

<span data-ttu-id="acfd3-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acfd3-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="acfd3-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acfd3-111">Properties</span></span>

<span data-ttu-id="acfd3-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="acfd3-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="acfd3-113">Relações</span><span class="sxs-lookup"><span data-stu-id="acfd3-113">Relationships</span></span>

<span data-ttu-id="acfd3-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="acfd3-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="acfd3-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="acfd3-115">Methods</span></span>

| <span data-ttu-id="acfd3-116">Método</span><span class="sxs-lookup"><span data-stu-id="acfd3-116">Method</span></span>       | <span data-ttu-id="acfd3-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="acfd3-117">Return Type</span></span> | <span data-ttu-id="acfd3-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="acfd3-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="acfd3-119">query</span><span class="sxs-lookup"><span data-stu-id="acfd3-119">query</span></span>](../api/search-query.md) | [<span data-ttu-id="acfd3-120">searchResponse</span><span class="sxs-lookup"><span data-stu-id="acfd3-120">searchResponse</span></span>](searchresponse.md)| <span data-ttu-id="acfd3-121">Executa a consulta especificada no [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="acfd3-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


