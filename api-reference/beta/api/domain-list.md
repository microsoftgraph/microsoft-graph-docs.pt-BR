---
title: Listar domínios
description: Recupere uma lista de objetos Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c0a41b7ec7d0bbacfb61b8d274c972dd891fa1af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321172"
---
# <a name="list-domains"></a><span data-ttu-id="5415a-103">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="5415a-103">List domains</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5415a-104">Recupere uma lista de objetos Domain.</span><span class="sxs-lookup"><span data-stu-id="5415a-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5415a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5415a-105">Permissions</span></span>
<span data-ttu-id="5415a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5415a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5415a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5415a-108">Permission type</span></span>      | <span data-ttu-id="5415a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5415a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5415a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5415a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5415a-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5415a-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="5415a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5415a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5415a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5415a-113">Not supported.</span></span>    |
|<span data-ttu-id="5415a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5415a-114">Application</span></span> | <span data-ttu-id="5415a-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5415a-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5415a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5415a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5415a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5415a-117">Optional query parameters</span></span>
<span data-ttu-id="5415a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5415a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5415a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5415a-119">Request headers</span></span>
| <span data-ttu-id="5415a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5415a-120">Name</span></span>      |<span data-ttu-id="5415a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5415a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5415a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5415a-122">Authorization</span></span>  | <span data-ttu-id="5415a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5415a-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5415a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5415a-125">Accept</span></span>         | <span data-ttu-id="5415a-126">Application/JSON;</span><span class="sxs-lookup"><span data-stu-id="5415a-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="5415a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5415a-127">Request body</span></span>
<span data-ttu-id="5415a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5415a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5415a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5415a-129">Response</span></span>

<span data-ttu-id="5415a-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5415a-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5415a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5415a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5415a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5415a-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5415a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5415a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5415a-134">C#</span><span class="sxs-lookup"><span data-stu-id="5415a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5415a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5415a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5415a-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5415a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5415a-137">Java</span><span class="sxs-lookup"><span data-stu-id="5415a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5415a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5415a-138">Response</span></span>
<span data-ttu-id="5415a-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5415a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "name": "contoso.com",
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
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
