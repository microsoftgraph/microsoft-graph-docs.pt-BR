---
title: Criar activityBasedTimeoutPolicy
description: Criar um novo activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 670e912edd8cc966d0fbc07247ffcd6e3cbeffa0
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917119"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="1f14f-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="1f14f-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="1f14f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f14f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1f14f-105">Criar um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1f14f-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f14f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f14f-106">Permissions</span></span>

<span data-ttu-id="1f14f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f14f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f14f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f14f-109">Permission type</span></span>                        | <span data-ttu-id="1f14f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f14f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f14f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f14f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f14f-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f14f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1f14f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f14f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f14f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f14f-114">Not supported.</span></span> |
| <span data-ttu-id="1f14f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f14f-115">Application</span></span>                            | <span data-ttu-id="1f14f-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f14f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f14f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f14f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1f14f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f14f-118">Request headers</span></span>

| <span data-ttu-id="1f14f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1f14f-119">Name</span></span>          | <span data-ttu-id="1f14f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f14f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1f14f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f14f-121">Authorization</span></span> | <span data-ttu-id="1f14f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f14f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f14f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1f14f-124">Content-type</span></span> | <span data-ttu-id="1f14f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f14f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f14f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f14f-127">Request body</span></span>

<span data-ttu-id="1f14f-128">No corpo da solicitação, forneça uma representação JSON de um objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1f14f-128">In the request body, supply a JSON representation of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1f14f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f14f-129">Response</span></span>

<span data-ttu-id="1f14f-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f14f-130">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f14f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1f14f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f14f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f14f-132">Request</span></span>

<span data-ttu-id="1f14f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f14f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f14f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f14f-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1f14f-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f14f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f14f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f14f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f14f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f14f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f14f-138">Java</span><span class="sxs-lookup"><span data-stu-id="1f14f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f14f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f14f-139">Response</span></span>

<span data-ttu-id="1f14f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f14f-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1f14f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f14f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
