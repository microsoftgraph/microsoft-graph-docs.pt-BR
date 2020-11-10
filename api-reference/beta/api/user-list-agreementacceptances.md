---
title: Listar agreementAcceptances
description: Recupere uma lista de objetos agreementAcceptance de um usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 3e7f256b5fb800a17a8d329463f44a5ddc571f33
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973808"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="9cf84-103">Listar agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="9cf84-103">List agreementAcceptances</span></span>

<span data-ttu-id="9cf84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf84-105">Recupere uma lista de objetos [agreementAcceptance](../resources/agreementacceptance.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9cf84-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cf84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cf84-106">Permissions</span></span>
<span data-ttu-id="9cf84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cf84-109">Permission type</span></span>                        | <span data-ttu-id="9cf84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cf84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cf84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cf84-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cf84-112">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="9cf84-112">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="9cf84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cf84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cf84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cf84-114">Not supported.</span></span> |
|<span data-ttu-id="9cf84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cf84-115">Application</span></span>                            | <span data-ttu-id="9cf84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cf84-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cf84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf84-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="9cf84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf84-118">Request headers</span></span>
| <span data-ttu-id="9cf84-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9cf84-119">Name</span></span>      |<span data-ttu-id="9cf84-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf84-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cf84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cf84-121">Authorization</span></span> | <span data-ttu-id="9cf84-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9cf84-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cf84-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf84-123">Request body</span></span>
<span data-ttu-id="9cf84-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cf84-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9cf84-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf84-125">Response</span></span>
<span data-ttu-id="9cf84-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf84-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cf84-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cf84-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cf84-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf84-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9cf84-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf84-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="9cf84-130">C#</span><span class="sxs-lookup"><span data-stu-id="9cf84-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cf84-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cf84-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cf84-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cf84-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cf84-133">Java</span><span class="sxs-lookup"><span data-stu-id="9cf84-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9cf84-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf84-134">Response</span></span>
><span data-ttu-id="9cf84-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cf84-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
