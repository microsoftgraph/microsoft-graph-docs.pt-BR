---
title: Obter domínio
description: Recupere as propriedades e as relações do objeto domain.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e7118d376aa403d43eeeef1d8888984fea6c9ca0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448531"
---
# <a name="get-domain"></a><span data-ttu-id="b8d50-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="b8d50-103">Get domain</span></span>

<span data-ttu-id="b8d50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8d50-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8d50-105">Recupere as propriedades e as relações do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="b8d50-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8d50-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8d50-106">Permissions</span></span>

<span data-ttu-id="b8d50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8d50-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8d50-109">Permission type</span></span>      | <span data-ttu-id="b8d50-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8d50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8d50-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8d50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b8d50-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d50-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="b8d50-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8d50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8d50-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8d50-114">Not supported.</span></span>    |
|<span data-ttu-id="b8d50-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8d50-115">Application</span></span> | <span data-ttu-id="b8d50-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d50-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8d50-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d50-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="b8d50-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="b8d50-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b8d50-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8d50-119">Optional query parameters</span></span>

<span data-ttu-id="b8d50-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d50-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8d50-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d50-121">Request headers</span></span>

| <span data-ttu-id="b8d50-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b8d50-122">Name</span></span>      |<span data-ttu-id="b8d50-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8d50-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8d50-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8d50-124">Authorization</span></span>  | <span data-ttu-id="b8d50-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8d50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8d50-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8d50-127">Content-Type</span></span>  | <span data-ttu-id="b8d50-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b8d50-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8d50-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d50-129">Request body</span></span>
<span data-ttu-id="b8d50-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8d50-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8d50-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d50-131">Response</span></span>

<span data-ttu-id="b8d50-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um](../resources/domain.md) objeto de domínio no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d50-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8d50-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8d50-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8d50-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d50-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b8d50-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d50-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="b8d50-136">C#</span><span class="sxs-lookup"><span data-stu-id="b8d50-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8d50-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8d50-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8d50-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8d50-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8d50-139">Java</span><span class="sxs-lookup"><span data-stu-id="b8d50-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8d50-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d50-140">Response</span></span>
<span data-ttu-id="b8d50-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8d50-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
