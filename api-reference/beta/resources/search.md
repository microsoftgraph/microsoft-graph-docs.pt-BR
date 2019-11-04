---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 65a099ea0ae57b116bcf6a251170e507945226c9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938769"
---
# <a name="search-resource-type"></a><span data-ttu-id="dcf20-103">tipo de recurso de pesquisa</span><span class="sxs-lookup"><span data-stu-id="dcf20-103">search resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf20-104">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dcf20-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="dcf20-105">Ele serve como uma âncora para a ação de [consulta](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="dcf20-105">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="dcf20-106">Esse recurso não deve ser chamado como tal.</span><span class="sxs-lookup"><span data-stu-id="dcf20-106">This resource is not expected to be called as such.</span></span> <span data-ttu-id="dcf20-107">Qualquer solicitação no recurso causará uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="dcf20-107">Any request on the resource will incur a Bad Request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcf20-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dcf20-108">JSON representation</span></span>

<span data-ttu-id="dcf20-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dcf20-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="dcf20-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dcf20-110">Properties</span></span>

<span data-ttu-id="dcf20-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dcf20-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dcf20-112">Relações</span><span class="sxs-lookup"><span data-stu-id="dcf20-112">Relationships</span></span>

<span data-ttu-id="dcf20-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dcf20-113">None</span></span>

## <a name="methods"></a><span data-ttu-id="dcf20-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="dcf20-114">Methods</span></span>

| <span data-ttu-id="dcf20-115">Método</span><span class="sxs-lookup"><span data-stu-id="dcf20-115">Method</span></span>       | <span data-ttu-id="dcf20-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dcf20-116">Return Type</span></span> | <span data-ttu-id="dcf20-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcf20-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dcf20-118">Query</span><span class="sxs-lookup"><span data-stu-id="dcf20-118">query</span></span>](../api/search-query.md) | <span data-ttu-id="dcf20-119">[searchResponse](searchresponse.md) Coletânea</span><span class="sxs-lookup"><span data-stu-id="dcf20-119">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="dcf20-120">Executa a consulta especificada no [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="dcf20-120">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
