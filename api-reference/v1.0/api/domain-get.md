---
title: Obter domínio
description: Recupere as propriedades e as relações do objeto domain.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5ff05e7df119afe6d858453d65a3db29de8ee0d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052422"
---
# <a name="get-domain"></a><span data-ttu-id="2b9b9-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="2b9b9-103">Get domain</span></span>

<span data-ttu-id="2b9b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b9b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b9b9-105">Recupere as propriedades e as relações do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b9b9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b9b9-106">Permissions</span></span>

<span data-ttu-id="2b9b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b9b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b9b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b9b9-109">Permission type</span></span>      | <span data-ttu-id="2b9b9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b9b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b9b9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b9b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b9b9-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b9b9-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="2b9b9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b9b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b9b9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-114">Not supported.</span></span>    |
|<span data-ttu-id="2b9b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b9b9-115">Application</span></span> | <span data-ttu-id="2b9b9-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b9b9-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b9b9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b9b9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="2b9b9-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2b9b9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b9b9-119">Optional query parameters</span></span>

<span data-ttu-id="2b9b9-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b9b9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b9b9-121">Request headers</span></span>

| <span data-ttu-id="2b9b9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2b9b9-122">Name</span></span>      |<span data-ttu-id="2b9b9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b9b9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b9b9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b9b9-124">Authorization</span></span>  | <span data-ttu-id="2b9b9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b9b9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b9b9-127">Content-Type</span></span>  | <span data-ttu-id="2b9b9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2b9b9-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b9b9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b9b9-129">Request body</span></span>
<span data-ttu-id="2b9b9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b9b9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b9b9-131">Response</span></span>

<span data-ttu-id="2b9b9-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um](../resources/domain.md) objeto de domínio no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b9b9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b9b9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b9b9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b9b9-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2b9b9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b9b9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="2b9b9-136">C#</span><span class="sxs-lookup"><span data-stu-id="2b9b9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b9b9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b9b9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b9b9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b9b9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b9b9-139">Java</span><span class="sxs-lookup"><span data-stu-id="2b9b9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b9b9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b9b9-140">Response</span></span>
<span data-ttu-id="2b9b9-141">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2b9b9-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
