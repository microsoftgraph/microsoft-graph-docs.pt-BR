---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a30a1fe5891a0f8a58f08d742ef2aac645006156
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985781"
---
# <a name="search-resource-type"></a><span data-ttu-id="55e8e-103">tipo de recurso de pesquisa</span><span class="sxs-lookup"><span data-stu-id="55e8e-103">search resource type</span></span>

<span data-ttu-id="55e8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55e8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e8e-105">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="55e8e-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="55e8e-106">Ele serve como uma âncora para a ação de [consulta](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="55e8e-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="55e8e-107">Esse recurso não deve ser chamado como tal.</span><span class="sxs-lookup"><span data-stu-id="55e8e-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="55e8e-108">Qualquer solicitação no recurso causará uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="55e8e-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="55e8e-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55e8e-109">JSON representation</span></span>

<span data-ttu-id="55e8e-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55e8e-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="55e8e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55e8e-111">Properties</span></span>

<span data-ttu-id="55e8e-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="55e8e-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="55e8e-113">Relações</span><span class="sxs-lookup"><span data-stu-id="55e8e-113">Relationships</span></span>

<span data-ttu-id="55e8e-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="55e8e-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="55e8e-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="55e8e-115">Methods</span></span>

| <span data-ttu-id="55e8e-116">Método</span><span class="sxs-lookup"><span data-stu-id="55e8e-116">Method</span></span>       | <span data-ttu-id="55e8e-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="55e8e-117">Return Type</span></span> | <span data-ttu-id="55e8e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="55e8e-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="55e8e-119">query</span><span class="sxs-lookup"><span data-stu-id="55e8e-119">query</span></span>](../api/search-query.md) | <span data-ttu-id="55e8e-120">[searchResponse](searchresponse.md) Coletânea</span><span class="sxs-lookup"><span data-stu-id="55e8e-120">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="55e8e-121">Executa a consulta especificada no [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="55e8e-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


