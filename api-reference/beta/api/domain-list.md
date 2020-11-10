---
title: Listar domínios
description: Recupere uma lista de objetos Domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0e126ef4a46628d725cb3c9672bf5f9bcd0ef888
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963921"
---
# <a name="list-domains"></a><span data-ttu-id="ec575-103">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="ec575-103">List domains</span></span>

<span data-ttu-id="ec575-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec575-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec575-105">Recupere uma lista de objetos Domain.</span><span class="sxs-lookup"><span data-stu-id="ec575-105">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec575-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec575-106">Permissions</span></span>
<span data-ttu-id="ec575-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec575-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec575-109">Permission type</span></span>      | <span data-ttu-id="ec575-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec575-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec575-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec575-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec575-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec575-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="ec575-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec575-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec575-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec575-114">Not supported.</span></span>    |
|<span data-ttu-id="ec575-115">Application</span><span class="sxs-lookup"><span data-stu-id="ec575-115">Application</span></span> | <span data-ttu-id="ec575-116">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec575-116">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec575-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec575-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec575-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec575-118">Optional query parameters</span></span>
<span data-ttu-id="ec575-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec575-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec575-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec575-120">Request headers</span></span>
| <span data-ttu-id="ec575-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ec575-121">Name</span></span>      |<span data-ttu-id="ec575-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec575-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec575-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec575-123">Authorization</span></span>  | <span data-ttu-id="ec575-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec575-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ec575-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec575-126">Accept</span></span>         | <span data-ttu-id="ec575-127">Application/JSON;</span><span class="sxs-lookup"><span data-stu-id="ec575-127">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec575-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec575-128">Request body</span></span>
<span data-ttu-id="ec575-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec575-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec575-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec575-130">Response</span></span>

<span data-ttu-id="ec575-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec575-131">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec575-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec575-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec575-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec575-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec575-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec575-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains
```
# <a name="c"></a>[<span data-ttu-id="ec575-135">C#</span><span class="sxs-lookup"><span data-stu-id="ec575-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec575-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec575-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec575-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec575-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec575-138">Java</span><span class="sxs-lookup"><span data-stu-id="ec575-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec575-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec575-139">Response</span></span>
<span data-ttu-id="ec575-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec575-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
