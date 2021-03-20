---
title: Listar agreementAcceptances
description: Recupere uma lista de objetos agreementAcceptance de um usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 178e6afe9b9bd62e1f921f6ddc6c3c9148c57cb9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943686"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="0d673-103">Listar agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="0d673-103">List agreementAcceptances</span></span>

<span data-ttu-id="0d673-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d673-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d673-105">Recupere uma lista de objetos [agreementAcceptance de um](../resources/agreementacceptance.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="0d673-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d673-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d673-106">Permissions</span></span>
<span data-ttu-id="0d673-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d673-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d673-109">Permission type</span></span>                        | <span data-ttu-id="0d673-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d673-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d673-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d673-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d673-112">AgreementAcceptance.Read, AgreementAcceptance.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d673-112">AgreementAcceptance.Read, AgreementAcceptance.Read.All</span></span> |
|<span data-ttu-id="0d673-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d673-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d673-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d673-114">Not supported.</span></span> |
|<span data-ttu-id="0d673-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d673-115">Application</span></span>                            | <span data-ttu-id="0d673-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d673-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d673-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d673-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="0d673-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d673-118">Request headers</span></span>
| <span data-ttu-id="0d673-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0d673-119">Name</span></span>      |<span data-ttu-id="0d673-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d673-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d673-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d673-121">Authorization</span></span> | <span data-ttu-id="0d673-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0d673-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d673-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d673-123">Request body</span></span>
<span data-ttu-id="0d673-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d673-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0d673-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d673-125">Response</span></span>
<span data-ttu-id="0d673-126">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d673-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d673-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d673-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d673-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d673-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0d673-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d673-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="0d673-130">C#</span><span class="sxs-lookup"><span data-stu-id="0d673-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d673-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d673-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d673-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d673-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d673-133">Java</span><span class="sxs-lookup"><span data-stu-id="0d673-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0d673-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d673-134">Response</span></span>
><span data-ttu-id="0d673-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d673-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
