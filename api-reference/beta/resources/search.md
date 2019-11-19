---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bb38d281895ac11d97a026a4352f68b93e8ba801
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704059"
---
# <a name="search-resource-type"></a><span data-ttu-id="4abd5-103">tipo de recurso de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4abd5-103">search resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4abd5-104">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4abd5-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="4abd5-105">Ele serve como uma âncora para a ação de [consulta](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="4abd5-105">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="4abd5-106">Esse recurso não deve ser chamado como tal.</span><span class="sxs-lookup"><span data-stu-id="4abd5-106">This resource is not expected to be called as such.</span></span> <span data-ttu-id="4abd5-107">Qualquer solicitação no recurso causará uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="4abd5-107">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="4abd5-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4abd5-108">JSON representation</span></span>

<span data-ttu-id="4abd5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4abd5-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="4abd5-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4abd5-110">Properties</span></span>

<span data-ttu-id="4abd5-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4abd5-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4abd5-112">Relações</span><span class="sxs-lookup"><span data-stu-id="4abd5-112">Relationships</span></span>

<span data-ttu-id="4abd5-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4abd5-113">None</span></span>

## <a name="methods"></a><span data-ttu-id="4abd5-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="4abd5-114">Methods</span></span>

| <span data-ttu-id="4abd5-115">Método</span><span class="sxs-lookup"><span data-stu-id="4abd5-115">Method</span></span>       | <span data-ttu-id="4abd5-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4abd5-116">Return Type</span></span> | <span data-ttu-id="4abd5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4abd5-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4abd5-118">query</span><span class="sxs-lookup"><span data-stu-id="4abd5-118">query</span></span>](../api/search-query.md) | <span data-ttu-id="4abd5-119">[searchResponse](searchresponse.md) Coletânea</span><span class="sxs-lookup"><span data-stu-id="4abd5-119">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="4abd5-120">Executa a consulta especificada no [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="4abd5-120">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
