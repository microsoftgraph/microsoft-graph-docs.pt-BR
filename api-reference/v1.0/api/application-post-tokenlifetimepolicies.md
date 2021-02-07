---
title: Atribiur tokenLifetimePolicy
description: Atribua um tokenLifetimePolicy a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1d32530e70e1e08bda153ec83c459722eee0da1b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131765"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="f2dea-103">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f2dea-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="f2dea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2dea-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f2dea-105">Atribua [um tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) a um [aplicativo.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="f2dea-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2dea-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2dea-106">Permissions</span></span>

<span data-ttu-id="f2dea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2dea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2dea-109">Permission type</span></span>                        | <span data-ttu-id="f2dea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2dea-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2dea-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2dea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2dea-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2dea-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="f2dea-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2dea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2dea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2dea-114">Not supported.</span></span> |
| <span data-ttu-id="f2dea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2dea-115">Application</span></span>                            | <span data-ttu-id="f2dea-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2dea-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2dea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2dea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f2dea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dea-118">Request headers</span></span>

| <span data-ttu-id="f2dea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f2dea-119">Name</span></span>          | <span data-ttu-id="f2dea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dea-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f2dea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2dea-121">Authorization</span></span> | <span data-ttu-id="f2dea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2dea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2dea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2dea-124">Content-Type</span></span> | <span data-ttu-id="f2dea-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2dea-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2dea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dea-127">Request body</span></span>

<span data-ttu-id="f2dea-128">No corpo da solicitação, fornece o identificador do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) (usando uma propriedade) que deve ser atribuído ao aplicativo ou entidade `@odata.id` de serviço.</span><span class="sxs-lookup"><span data-stu-id="f2dea-128">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="f2dea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2dea-129">Response</span></span>

<span data-ttu-id="f2dea-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2dea-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2dea-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2dea-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2dea-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dea-133">Request</span></span>

<span data-ttu-id="f2dea-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2dea-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2dea-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2dea-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="f2dea-136">C#</span><span class="sxs-lookup"><span data-stu-id="f2dea-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2dea-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2dea-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2dea-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2dea-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2dea-139">Java</span><span class="sxs-lookup"><span data-stu-id="f2dea-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2dea-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2dea-140">Response</span></span>

<span data-ttu-id="f2dea-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2dea-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

