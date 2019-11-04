---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d7b84fdad96530f88f09c7da7b00a6013b19017e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938383"
---
# <a name="search"></a><span data-ttu-id="6745a-103">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="6745a-103">Search</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6745a-104">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6745a-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="6745a-105">Ela não se comporta como qualquer outro recurso no Graph, mas serve como uma âncora para ações de pesquisa (consulta).</span><span class="sxs-lookup"><span data-stu-id="6745a-105">It does not behave as any other resource in Graph, but serves as an anchor to Search actions (Query).</span></span> <span data-ttu-id="6745a-106">Ele não tem representação de recurso no gráfico.</span><span class="sxs-lookup"><span data-stu-id="6745a-106">It has no resource representation in graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="6745a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6745a-107">Permissions</span></span>

<span data-ttu-id="6745a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6745a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6745a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6745a-110">Permission type</span></span>                        | <span data-ttu-id="6745a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6745a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6745a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6745a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6745a-113">Mail. Read, files. Read. All, Calendars. Read, ExternalItem. Read. All</span><span class="sxs-lookup"><span data-stu-id="6745a-113">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="6745a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6745a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6745a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6745a-115">Not supported.</span></span> |
| <span data-ttu-id="6745a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6745a-116">Application</span></span>                            | <span data-ttu-id="6745a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6745a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6745a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6745a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a><span data-ttu-id="6745a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6745a-119">Request headers</span></span>

| <span data-ttu-id="6745a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6745a-120">Name</span></span>      |<span data-ttu-id="6745a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6745a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6745a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6745a-122">Authorization</span></span> | <span data-ttu-id="6745a-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6745a-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6745a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6745a-124">Request body</span></span>

<span data-ttu-id="6745a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6745a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6745a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6745a-126">Response</span></span>

<span data-ttu-id="6745a-127">Esse recurso não deve ser chamado como tal.</span><span class="sxs-lookup"><span data-stu-id="6745a-127">This resource is not expected to be called as such.</span></span> <span data-ttu-id="6745a-128">Qualquer solicitação no recurso causará uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="6745a-128">Any request on the resource will incur a Bad Request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6745a-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6745a-129">Next steps</span></span>

- <span data-ttu-id="6745a-130">Explore a ação [/Query](search-query.md) na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6745a-130">Explore the [/query](search-query.md) action on Search.</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
