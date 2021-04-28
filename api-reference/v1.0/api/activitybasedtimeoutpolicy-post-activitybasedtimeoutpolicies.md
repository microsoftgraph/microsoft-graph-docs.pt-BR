---
title: Criar activityBasedTimeoutPolicy
description: Crie uma nova activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 552dc8688bd21149ecc868fe7af658760eb9f4d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054228"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="ec770-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ec770-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="ec770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec770-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ec770-105">Crie um novo [objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec770-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec770-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec770-106">Permissions</span></span>

<span data-ttu-id="ec770-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec770-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec770-109">Permission type</span></span>                        | <span data-ttu-id="ec770-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec770-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec770-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec770-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec770-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec770-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ec770-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec770-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec770-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec770-114">Not supported.</span></span> |
| <span data-ttu-id="ec770-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec770-115">Application</span></span>                            | <span data-ttu-id="ec770-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec770-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec770-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec770-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ec770-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec770-118">Request headers</span></span>

| <span data-ttu-id="ec770-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ec770-119">Name</span></span>          | <span data-ttu-id="ec770-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec770-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ec770-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec770-121">Authorization</span></span> | <span data-ttu-id="ec770-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec770-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec770-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ec770-124">Content-type</span></span> | <span data-ttu-id="ec770-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec770-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec770-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec770-127">Request body</span></span>

<span data-ttu-id="ec770-128">No corpo da solicitação, fornece uma representação JSON de [um objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec770-128">In the request body, supply a JSON representation of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec770-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec770-129">Response</span></span>

<span data-ttu-id="ec770-130">Se tiver êxito, este método retornará um código de `201 Created` resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec770-130">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec770-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ec770-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec770-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec770-132">Request</span></span>

<span data-ttu-id="ec770-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec770-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ec770-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec770-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="ec770-135">C#</span><span class="sxs-lookup"><span data-stu-id="ec770-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec770-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec770-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec770-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec770-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec770-138">Java</span><span class="sxs-lookup"><span data-stu-id="ec770-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec770-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec770-139">Response</span></span>

<span data-ttu-id="ec770-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec770-140">The following is an example of the response.</span></span>

> <span data-ttu-id="ec770-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ec770-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

