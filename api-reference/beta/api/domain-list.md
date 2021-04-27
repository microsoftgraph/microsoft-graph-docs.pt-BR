---
title: Listar domínios
description: Recupere uma lista de objetos de domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6eeddc00a62efaa9b6432afe3d474b2f1019dfe6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046374"
---
# <a name="list-domains"></a><span data-ttu-id="c418c-103">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="c418c-103">List domains</span></span>

<span data-ttu-id="c418c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c418c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c418c-105">Recupere uma lista de objetos de domínio.</span><span class="sxs-lookup"><span data-stu-id="c418c-105">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c418c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c418c-106">Permissions</span></span>
<span data-ttu-id="c418c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c418c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c418c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c418c-109">Permission type</span></span>      | <span data-ttu-id="c418c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c418c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c418c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c418c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c418c-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c418c-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="c418c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c418c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c418c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c418c-114">Not supported.</span></span>    |
|<span data-ttu-id="c418c-115">Application</span><span class="sxs-lookup"><span data-stu-id="c418c-115">Application</span></span> | <span data-ttu-id="c418c-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c418c-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c418c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c418c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c418c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c418c-118">Optional query parameters</span></span>
<span data-ttu-id="c418c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c418c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c418c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c418c-120">Request headers</span></span>
| <span data-ttu-id="c418c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c418c-121">Name</span></span>      |<span data-ttu-id="c418c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c418c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c418c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c418c-123">Authorization</span></span>  | <span data-ttu-id="c418c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c418c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c418c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c418c-126">Accept</span></span>         | <span data-ttu-id="c418c-127">application/json;</span><span class="sxs-lookup"><span data-stu-id="c418c-127">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="c418c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c418c-128">Request body</span></span>
<span data-ttu-id="c418c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c418c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c418c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c418c-130">Response</span></span>

<span data-ttu-id="c418c-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/domain.md) domínio no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c418c-131">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c418c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c418c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c418c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c418c-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c418c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c418c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains
```
# <a name="c"></a>[<span data-ttu-id="c418c-135">C#</span><span class="sxs-lookup"><span data-stu-id="c418c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c418c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c418c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c418c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c418c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c418c-138">Java</span><span class="sxs-lookup"><span data-stu-id="c418c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c418c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c418c-139">Response</span></span>
<span data-ttu-id="c418c-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c418c-140">Note: The response object shown here might be shortened for readability.</span></span>
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
