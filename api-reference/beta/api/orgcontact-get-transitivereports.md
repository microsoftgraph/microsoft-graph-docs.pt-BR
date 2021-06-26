---
title: Obter transitiveReports para orgContact
description: Obter a contagem de relatórios transitivos para um contato organizacional.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43a3d7736d33a1ca21ccf881dba92275dde553a8
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151766"
---
# <a name="get-transitivereports-for-orgcontact"></a><span data-ttu-id="c75c3-103">Obter transitiveReports para orgContact</span><span class="sxs-lookup"><span data-stu-id="c75c3-103">Get transitiveReports for orgContact</span></span>

<span data-ttu-id="c75c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c75c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c75c3-105">Recupere uma contagem de relatórios transitivos para um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="c75c3-105">Retrieve a count of transitive reports for an organizational contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="c75c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c75c3-106">Permissions</span></span>

<span data-ttu-id="c75c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c75c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="c75c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c75c3-109">Permission type</span></span> | <span data-ttu-id="c75c3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c75c3-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="c75c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c75c3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c75c3-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c75c3-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="c75c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c75c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c75c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c75c3-114">Not supported.</span></span> |
| <span data-ttu-id="c75c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c75c3-115">Application</span></span> | <span data-ttu-id="c75c3-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c75c3-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c75c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c75c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/transitiveReports/$count
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c75c3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c75c3-118">Optional query parameters</span></span>

<span data-ttu-id="c75c3-119">Esse método não dá suporte ao uso de parâmetros de consulta, mas exige `$count` o segmento de consulta.</span><span class="sxs-lookup"><span data-stu-id="c75c3-119">This method does not support the use of query parameters, but does require the `$count` query segment.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c75c3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c75c3-120">Request headers</span></span>

| <span data-ttu-id="c75c3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c75c3-121">Header</span></span>       | <span data-ttu-id="c75c3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c75c3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c75c3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c75c3-123">Authorization</span></span>  | <span data-ttu-id="c75c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c75c3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c75c3-126">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c75c3-126">ConsistencyLevel</span></span> | <span data-ttu-id="c75c3-127">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="c75c3-127">eventual.</span></span> <span data-ttu-id="c75c3-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c75c3-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c75c3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c75c3-129">Request body</span></span>

<span data-ttu-id="c75c3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c75c3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c75c3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c75c3-131">Response</span></span>

<span data-ttu-id="c75c3-132">Se tiver êxito, este método retornará um código de resposta e uma contagem de relatórios `200 OK` transitivos para um contato organizacional no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c75c3-132">If successful, this method returns a `200 OK` response code and a count of transitive reports for an organizational contact in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c75c3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c75c3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c75c3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c75c3-134">Request</span></span>

<span data-ttu-id="c75c3-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c75c3-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivereports"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```

### <a name="response"></a><span data-ttu-id="c75c3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c75c3-136">Response</span></span>

<span data-ttu-id="c75c3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c75c3-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="c75c3-138">5 </span><span class="sxs-lookup"><span data-stu-id="c75c3-138">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
