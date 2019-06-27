---
title: Listar agreementAcceptances
description: Recupere uma lista de objetos agreementAcceptance de um usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8ca6788bec02713131aaa6006e4327b85e85eff0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270298"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="2c3e1-103">Listar agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="2c3e1-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c3e1-104">Recupere uma lista de objetos [agreementAcceptance](../resources/agreementacceptance.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2c3e1-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c3e1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c3e1-105">Permissions</span></span>
<span data-ttu-id="2c3e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c3e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c3e1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c3e1-108">Permission type</span></span>                        | <span data-ttu-id="2c3e1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c3e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c3e1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c3e1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c3e1-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="2c3e1-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="2c3e1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c3e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c3e1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c3e1-113">Not supported.</span></span> |
|<span data-ttu-id="2c3e1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c3e1-114">Application</span></span>                            | <span data-ttu-id="2c3e1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c3e1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c3e1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c3e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="2c3e1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c3e1-117">Request headers</span></span>
| <span data-ttu-id="2c3e1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2c3e1-118">Name</span></span>      |<span data-ttu-id="2c3e1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c3e1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c3e1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c3e1-120">Authorization</span></span> | <span data-ttu-id="2c3e1-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2c3e1-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c3e1-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c3e1-122">Request body</span></span>
<span data-ttu-id="2c3e1-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c3e1-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2c3e1-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c3e1-124">Response</span></span>
<span data-ttu-id="2c3e1-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c3e1-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c3e1-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c3e1-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c3e1-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c3e1-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="2c3e1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c3e1-128">Response</span></span>
><span data-ttu-id="2c3e1-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c3e1-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c3e1-131">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c3e1-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c3e1-132">C#</span><span class="sxs-lookup"><span data-stu-id="2c3e1-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c3e1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c3e1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c3e1-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c3e1-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
