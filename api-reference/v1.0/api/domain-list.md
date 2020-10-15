---
title: Listar domínios
description: Recupere uma lista de objetos Domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c275ea7a0811a05d5bee028aa5cbf645cdc832ab
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461360"
---
# <a name="list-domains"></a><span data-ttu-id="9d43a-103">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="9d43a-103">List domains</span></span>

<span data-ttu-id="9d43a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d43a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d43a-105">Recupere uma lista de objetos Domain.</span><span class="sxs-lookup"><span data-stu-id="9d43a-105">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d43a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d43a-106">Permissions</span></span>
<span data-ttu-id="9d43a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d43a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d43a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d43a-109">Permission type</span></span>      | <span data-ttu-id="9d43a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d43a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d43a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d43a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d43a-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d43a-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="9d43a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d43a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d43a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d43a-114">Not supported.</span></span>    |
|<span data-ttu-id="9d43a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d43a-115">Application</span></span> | <span data-ttu-id="9d43a-116">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d43a-116">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d43a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d43a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d43a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d43a-118">Optional query parameters</span></span>
<span data-ttu-id="9d43a-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d43a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d43a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d43a-120">Request headers</span></span>
| <span data-ttu-id="9d43a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9d43a-121">Name</span></span>      |<span data-ttu-id="9d43a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d43a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d43a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d43a-123">Authorization</span></span>  | <span data-ttu-id="9d43a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d43a-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9d43a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d43a-126">Accept</span></span>         | <span data-ttu-id="9d43a-127">Application/JSON;</span><span class="sxs-lookup"><span data-stu-id="9d43a-127">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d43a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d43a-128">Request body</span></span>
<span data-ttu-id="9d43a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d43a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d43a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d43a-130">Response</span></span>

<span data-ttu-id="9d43a-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d43a-131">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d43a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d43a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d43a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d43a-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9d43a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d43a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains
```
# <a name="c"></a>[<span data-ttu-id="9d43a-135">C#</span><span class="sxs-lookup"><span data-stu-id="9d43a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d43a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d43a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d43a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d43a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d43a-138">Java</span><span class="sxs-lookup"><span data-stu-id="9d43a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9d43a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d43a-139">Response</span></span>
<span data-ttu-id="9d43a-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d43a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
