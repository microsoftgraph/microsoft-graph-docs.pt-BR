---
title: Listar agreementAcceptances
description: Recupere uma lista de objetos agreementAcceptance de um usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bbb2ef26989159cb7ff163aa5d7c79b6aba8e42e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451914"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="007e6-103">Listar agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="007e6-103">List agreementAcceptances</span></span>

<span data-ttu-id="007e6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="007e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="007e6-105">Recupere uma lista de objetos [agreementAcceptance](../resources/agreementacceptance.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="007e6-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="007e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="007e6-106">Permissions</span></span>
<span data-ttu-id="007e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="007e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="007e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="007e6-109">Permission type</span></span>                        | <span data-ttu-id="007e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="007e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="007e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="007e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="007e6-112">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="007e6-112">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="007e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="007e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="007e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="007e6-114">Not supported.</span></span> |
|<span data-ttu-id="007e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="007e6-115">Application</span></span>                            | <span data-ttu-id="007e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="007e6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="007e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="007e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="007e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="007e6-118">Request headers</span></span>
| <span data-ttu-id="007e6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="007e6-119">Name</span></span>      |<span data-ttu-id="007e6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="007e6-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="007e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="007e6-121">Authorization</span></span> | <span data-ttu-id="007e6-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="007e6-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="007e6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="007e6-123">Request body</span></span>
<span data-ttu-id="007e6-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="007e6-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="007e6-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="007e6-125">Response</span></span>
<span data-ttu-id="007e6-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="007e6-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="007e6-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="007e6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="007e6-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="007e6-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="007e6-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="007e6-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="007e6-130">C#</span><span class="sxs-lookup"><span data-stu-id="007e6-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="007e6-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="007e6-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="007e6-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="007e6-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="007e6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="007e6-133">Response</span></span>
><span data-ttu-id="007e6-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="007e6-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
