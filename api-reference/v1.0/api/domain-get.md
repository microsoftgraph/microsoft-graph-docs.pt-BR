---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 89f9fd1c8890af3cc0689a84bf6c2b90cfe27592
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016668"
---
# <a name="get-domain"></a><span data-ttu-id="2bc71-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="2bc71-103">Get domain</span></span>

<span data-ttu-id="2bc71-104">Recupere as propriedades e os relacionamentos do objeto Domain.</span><span class="sxs-lookup"><span data-stu-id="2bc71-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bc71-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2bc71-105">Permissions</span></span>

<span data-ttu-id="2bc71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bc71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2bc71-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bc71-108">Permission type</span></span>      | <span data-ttu-id="2bc71-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2bc71-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bc71-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bc71-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2bc71-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc71-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="2bc71-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bc71-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bc71-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bc71-113">Not supported.</span></span>    |
|<span data-ttu-id="2bc71-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bc71-114">Application</span></span> | <span data-ttu-id="2bc71-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc71-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bc71-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bc71-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="2bc71-117">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="2bc71-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2bc71-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bc71-118">Optional query parameters</span></span>

<span data-ttu-id="2bc71-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2bc71-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bc71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc71-120">Request headers</span></span>

| <span data-ttu-id="2bc71-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2bc71-121">Name</span></span>      |<span data-ttu-id="2bc71-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bc71-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2bc71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bc71-123">Authorization</span></span>  | <span data-ttu-id="2bc71-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bc71-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2bc71-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2bc71-126">Content-Type</span></span>  | <span data-ttu-id="2bc71-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2bc71-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bc71-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc71-128">Request body</span></span>
<span data-ttu-id="2bc71-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bc71-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc71-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc71-130">Response</span></span>

<span data-ttu-id="2bc71-131">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bc71-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bc71-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bc71-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bc71-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc71-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2bc71-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bc71-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2bc71-135">C#</span><span class="sxs-lookup"><span data-stu-id="2bc71-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2bc71-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="2bc71-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2bc71-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2bc71-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2bc71-138">Java</span><span class="sxs-lookup"><span data-stu-id="2bc71-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2bc71-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc71-139">Response</span></span>
<span data-ttu-id="2bc71-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bc71-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
