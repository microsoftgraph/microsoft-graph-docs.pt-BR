---
title: Obter presença
description: Obter informações de presença de um usuário.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: ccd05e056f4d751184dd2b5fbb9605377a9a64a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959676"
---
# <a name="get-presence"></a><span data-ttu-id="9770b-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="9770b-103">Get presence</span></span>

<span data-ttu-id="9770b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9770b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9770b-105">Obter informações de presença [de um](../resources/presence.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="9770b-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9770b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9770b-106">Permissions</span></span>
<span data-ttu-id="9770b-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="9770b-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="9770b-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9770b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9770b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9770b-109">Permission type</span></span> | <span data-ttu-id="9770b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9770b-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="9770b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9770b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9770b-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="9770b-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="9770b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9770b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9770b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9770b-114">Not Supported.</span></span>                        |
| <span data-ttu-id="9770b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9770b-115">Application</span></span>                            | <span data-ttu-id="9770b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9770b-116">Not Supported.</span></span>                        |

> <span data-ttu-id="9770b-117">**Observação:** A taxa máxima de solicitação para essa API é de 1500 solicitações de API em um período de 30 segundos, por aplicativo por locatário.</span><span class="sxs-lookup"><span data-stu-id="9770b-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="9770b-118">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="9770b-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="9770b-119">Headers de solicitação</span><span class="sxs-lookup"><span data-stu-id="9770b-119">Request Headers</span></span>
| <span data-ttu-id="9770b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9770b-120">Name</span></span>          | <span data-ttu-id="9770b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9770b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9770b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9770b-122">Authorization</span></span> | <span data-ttu-id="9770b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9770b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9770b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9770b-125">Request body</span></span>

<span data-ttu-id="9770b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9770b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9770b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9770b-127">Response</span></span>
<span data-ttu-id="9770b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [de](../resources/presence.md) presença no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9770b-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9770b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9770b-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="9770b-130">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="9770b-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="9770b-131">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="9770b-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="9770b-132">Esta operação requer a permissão Presence.Read.</span><span class="sxs-lookup"><span data-stu-id="9770b-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="9770b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9770b-133">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="9770b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9770b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```
# <a name="c"></a>[<span data-ttu-id="9770b-135">C#</span><span class="sxs-lookup"><span data-stu-id="9770b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9770b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9770b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9770b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9770b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9770b-138">Java</span><span class="sxs-lookup"><span data-stu-id="9770b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="9770b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9770b-139">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="9770b-140">Exemplo 2: Obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="9770b-140">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="9770b-141">O exemplo a seguir mostra como obter as informações de presença para outro usuário.</span><span class="sxs-lookup"><span data-stu-id="9770b-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="9770b-142">Esta operação requer a permissão Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="9770b-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="9770b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9770b-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9770b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9770b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="9770b-145">C#</span><span class="sxs-lookup"><span data-stu-id="9770b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9770b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9770b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9770b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9770b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9770b-148">Java</span><span class="sxs-lookup"><span data-stu-id="9770b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="9770b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9770b-149">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="9770b-150">Exemplo 3: Obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="9770b-150">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="9770b-151">O exemplo a seguir mostra como obter as informações de presença para outro usuário.</span><span class="sxs-lookup"><span data-stu-id="9770b-151">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="9770b-152">Esta operação requer a permissão Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="9770b-152">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="9770b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9770b-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9770b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9770b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="9770b-155">C#</span><span class="sxs-lookup"><span data-stu-id="9770b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9770b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9770b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9770b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9770b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9770b-158">Java</span><span class="sxs-lookup"><span data-stu-id="9770b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="9770b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="9770b-159">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


