---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8cb963c0fda545ea88e8d8e4335954ffb455102f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520932"
---
# <a name="search-resource-type"></a><span data-ttu-id="08352-103">tipo de recurso de pesquisa</span><span class="sxs-lookup"><span data-stu-id="08352-103">search resource type</span></span>

<span data-ttu-id="08352-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08352-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08352-105">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="08352-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="08352-106">Ele serve como uma âncora para a ação de [consulta](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="08352-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="08352-107">Esse recurso não deve ser chamado como tal.</span><span class="sxs-lookup"><span data-stu-id="08352-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="08352-108">Qualquer solicitação no recurso causará uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="08352-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="08352-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08352-109">JSON representation</span></span>

<span data-ttu-id="08352-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08352-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="08352-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08352-111">Properties</span></span>

<span data-ttu-id="08352-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="08352-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="08352-113">Relações</span><span class="sxs-lookup"><span data-stu-id="08352-113">Relationships</span></span>

<span data-ttu-id="08352-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08352-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="08352-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="08352-115">Methods</span></span>

| <span data-ttu-id="08352-116">Método</span><span class="sxs-lookup"><span data-stu-id="08352-116">Method</span></span>       | <span data-ttu-id="08352-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08352-117">Return Type</span></span> | <span data-ttu-id="08352-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="08352-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="08352-119">query</span><span class="sxs-lookup"><span data-stu-id="08352-119">query</span></span>](../api/search-query.md) | <span data-ttu-id="08352-120">[searchResponse](searchresponse.md) Coletânea</span><span class="sxs-lookup"><span data-stu-id="08352-120">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="08352-121">Executa a consulta especificada no [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="08352-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
