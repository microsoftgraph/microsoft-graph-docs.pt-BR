---
title: Obter transitiveReports para orgContact
description: Obter a contagem de relatórios transitivos para um contato organizacional.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e683e5224a3b473befea8f24c3971e5faf4a521
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210689"
---
# <a name="get-transitivereports-for-orgcontact"></a><span data-ttu-id="96354-103">Obter transitiveReports para orgContact</span><span class="sxs-lookup"><span data-stu-id="96354-103">Get transitiveReports for orgContact</span></span>

<span data-ttu-id="96354-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96354-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96354-105">Recupere uma contagem de relatórios transitivos para um contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="96354-105">Retrieve a count of transitive reports for an organizational contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="96354-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96354-106">Permissions</span></span>

<span data-ttu-id="96354-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="96354-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96354-109">Permission type</span></span> | <span data-ttu-id="96354-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96354-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="96354-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96354-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96354-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="96354-112">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="96354-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96354-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96354-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96354-114">Not supported.</span></span> |
| <span data-ttu-id="96354-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96354-115">Application</span></span> | <span data-ttu-id="96354-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="96354-116">OrgContact.Read, OrgContact.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96354-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96354-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/transitiveReports/$count
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96354-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96354-118">Optional query parameters</span></span>

<span data-ttu-id="96354-119">Esse método não dá suporte ao uso de parâmetros de consulta, mas exige `$count` o segmento de consulta.</span><span class="sxs-lookup"><span data-stu-id="96354-119">This method does not support the use of query parameters, but does require the `$count` query segment.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96354-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96354-120">Request headers</span></span>

| <span data-ttu-id="96354-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96354-121">Header</span></span>       | <span data-ttu-id="96354-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96354-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96354-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96354-123">Authorization</span></span>  | <span data-ttu-id="96354-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96354-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96354-126">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="96354-126">ConsistencyLevel</span></span> | <span data-ttu-id="96354-127">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="96354-127">eventual.</span></span> <span data-ttu-id="96354-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96354-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96354-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96354-129">Request body</span></span>

<span data-ttu-id="96354-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96354-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96354-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="96354-131">Response</span></span>

<span data-ttu-id="96354-132">Se tiver êxito, este método retornará um código de resposta e uma contagem de relatórios `200 OK` transitivos para um contato organizacional no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96354-132">If successful, this method returns a `200 OK` response code and a count of transitive reports for an organizational contact in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96354-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96354-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96354-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96354-134">Request</span></span>

<span data-ttu-id="96354-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96354-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96354-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="96354-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="96354-137">C#</span><span class="sxs-lookup"><span data-stu-id="96354-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96354-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96354-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96354-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96354-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96354-140">Java</span><span class="sxs-lookup"><span data-stu-id="96354-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96354-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="96354-141">Response</span></span>

<span data-ttu-id="96354-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96354-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="96354-143">5 </span><span class="sxs-lookup"><span data-stu-id="96354-143">5</span></span>

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
