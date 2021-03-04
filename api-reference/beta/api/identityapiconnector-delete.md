---
title: Excluir identityApiConnector
description: Exclui um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 74d8b44e73b6343efd55240e51bb22896e78ce6e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435606"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="ad4ce-103">Excluir identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ad4ce-103">Delete identityApiConnector</span></span>

<span data-ttu-id="ad4ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad4ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad4ce-105">Exclui um [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ad4ce-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad4ce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad4ce-106">Permissions</span></span>

<span data-ttu-id="ad4ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad4ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad4ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad4ce-109">Permission type</span></span>                        | <span data-ttu-id="ad4ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad4ce-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ad4ce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad4ce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad4ce-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4ce-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="ad4ce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad4ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad4ce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad4ce-114">Not supported.</span></span>  |
| <span data-ttu-id="ad4ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad4ce-115">Application</span></span>                            | <span data-ttu-id="ad4ce-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4ce-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="ad4ce-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ad4ce-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ad4ce-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ad4ce-118">Global administrator</span></span>
* <span data-ttu-id="ad4ce-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="ad4ce-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ad4ce-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad4ce-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="ad4ce-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad4ce-121">Request headers</span></span>
|<span data-ttu-id="ad4ce-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ad4ce-122">Name</span></span>|<span data-ttu-id="ad4ce-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad4ce-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ad4ce-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad4ce-124">Authorization</span></span>|<span data-ttu-id="ad4ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad4ce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad4ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad4ce-127">Request body</span></span>
<span data-ttu-id="ad4ce-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad4ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad4ce-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad4ce-129">Response</span></span>

<span data-ttu-id="ad4ce-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad4ce-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ad4ce-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ad4ce-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad4ce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad4ce-132">Request</span></span>

<span data-ttu-id="ad4ce-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad4ce-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad4ce-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad4ce-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="ad4ce-135">C#</span><span class="sxs-lookup"><span data-stu-id="ad4ce-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad4ce-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad4ce-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad4ce-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad4ce-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad4ce-138">Java</span><span class="sxs-lookup"><span data-stu-id="ad4ce-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad4ce-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad4ce-139">Response</span></span>

<span data-ttu-id="ad4ce-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad4ce-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
