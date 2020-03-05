---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 64e9c65d0de415e62d0238c58dc460dd1a82fcd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453705"
---
# <a name="search"></a><span data-ttu-id="c0f09-103">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="c0f09-103">Search</span></span>

<span data-ttu-id="c0f09-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c0f09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f09-105">O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c0f09-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="c0f09-106">Ela não se comporta como qualquer outro recurso no Graph, mas serve como uma âncora para ações de pesquisa (consulta).</span><span class="sxs-lookup"><span data-stu-id="c0f09-106">It does not behave as any other resource in Graph, but serves as an anchor to Search actions (Query).</span></span> <span data-ttu-id="c0f09-107">Ele não tem representação de recurso no gráfico.</span><span class="sxs-lookup"><span data-stu-id="c0f09-107">It has no resource representation in graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="c0f09-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0f09-108">Permissions</span></span>

<span data-ttu-id="c0f09-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0f09-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0f09-111">Permission type</span></span>                        | <span data-ttu-id="c0f09-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0f09-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0f09-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0f09-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0f09-114">Mail. Read, files. Read. All, Calendars. Read, ExternalItem. Read. All</span><span class="sxs-lookup"><span data-stu-id="c0f09-114">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="c0f09-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0f09-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f09-116">Not supported.</span></span> |
| <span data-ttu-id="c0f09-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0f09-117">Application</span></span>                            | <span data-ttu-id="c0f09-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f09-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0f09-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f09-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a><span data-ttu-id="c0f09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f09-120">Request headers</span></span>

| <span data-ttu-id="c0f09-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c0f09-121">Name</span></span>      |<span data-ttu-id="c0f09-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f09-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0f09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0f09-123">Authorization</span></span> | <span data-ttu-id="c0f09-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c0f09-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0f09-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f09-125">Request body</span></span>

<span data-ttu-id="c0f09-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0f09-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0f09-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f09-127">Response</span></span>

<span data-ttu-id="c0f09-128">Esse recurso não deve ser chamado como tal.</span><span class="sxs-lookup"><span data-stu-id="c0f09-128">This resource is not expected to be called as such.</span></span> <span data-ttu-id="c0f09-129">Qualquer solicitação no recurso causará uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="c0f09-129">Any request on the resource will incur a Bad Request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c0f09-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c0f09-130">Next steps</span></span>

- <span data-ttu-id="c0f09-131">Explore a ação [/Query](search-query.md) na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c0f09-131">Explore the [/query](search-query.md) action on Search.</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
