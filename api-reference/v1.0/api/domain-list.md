---
title: Listar domínios
description: Recupere uma lista de objetos Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da89c33876fe3ad70b4e25c223461480b0c4eb7a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721198"
---
# <a name="list-domains"></a><span data-ttu-id="b4c0b-103">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="b4c0b-103">List domains</span></span>

<span data-ttu-id="b4c0b-104">Recupere uma lista de objetos Domain.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4c0b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4c0b-105">Permissions</span></span>
<span data-ttu-id="b4c0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c0b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4c0b-108">Permission type</span></span>      | <span data-ttu-id="b4c0b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4c0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4c0b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4c0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4c0b-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4c0b-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="b4c0b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4c0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4c0b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-113">Not supported.</span></span>    |
|<span data-ttu-id="b4c0b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4c0b-114">Application</span></span> | <span data-ttu-id="b4c0b-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4c0b-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4c0b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4c0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4c0b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b4c0b-117">Optional query parameters</span></span>
<span data-ttu-id="b4c0b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4c0b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4c0b-119">Request headers</span></span>
| <span data-ttu-id="b4c0b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b4c0b-120">Name</span></span>      |<span data-ttu-id="b4c0b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4c0b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4c0b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4c0b-122">Authorization</span></span>  | <span data-ttu-id="b4c0b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b4c0b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4c0b-125">Accept</span></span>         | <span data-ttu-id="b4c0b-126">Application/JSON;</span><span class="sxs-lookup"><span data-stu-id="b4c0b-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4c0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4c0b-127">Request body</span></span>
<span data-ttu-id="b4c0b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4c0b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4c0b-129">Response</span></span>

<span data-ttu-id="b4c0b-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4c0b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4c0b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4c0b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4c0b-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4c0b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4c0b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4c0b-134">C#</span><span class="sxs-lookup"><span data-stu-id="b4c0b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4c0b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4c0b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4c0b-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b4c0b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4c0b-137">Java</span><span class="sxs-lookup"><span data-stu-id="b4c0b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b4c0b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4c0b-138">Response</span></span>
<span data-ttu-id="b4c0b-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4c0b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
