---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: f0b807775de40758514e5a839a3af1b1d3a20a01
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690553"
---
# <a name="get-presence"></a><span data-ttu-id="455a0-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="455a0-103">Get presence</span></span>

<span data-ttu-id="455a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="455a0-105">Obtenha as informações de [presença](../resources/presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="455a0-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="455a0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="455a0-106">Permissions</span></span>
<span data-ttu-id="455a0-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="455a0-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="455a0-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="455a0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="455a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="455a0-109">Permission type</span></span> | <span data-ttu-id="455a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="455a0-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="455a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="455a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="455a0-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="455a0-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="455a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="455a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="455a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="455a0-114">Not Supported.</span></span>                        |
| <span data-ttu-id="455a0-115">Application</span><span class="sxs-lookup"><span data-stu-id="455a0-115">Application</span></span>                            | <span data-ttu-id="455a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="455a0-116">Not Supported.</span></span>                        |

> <span data-ttu-id="455a0-117">**Observação:** A taxa máxima de solicitações para esta API são 1500 solicitações de API em um período de 30 segundos, por aplicativo por locatário.</span><span class="sxs-lookup"><span data-stu-id="455a0-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="455a0-118">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="455a0-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="455a0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="455a0-119">Request Headers</span></span>
| <span data-ttu-id="455a0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="455a0-120">Name</span></span>          | <span data-ttu-id="455a0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="455a0-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="455a0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="455a0-122">Authorization</span></span> | <span data-ttu-id="455a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="455a0-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="455a0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="455a0-125">Request body</span></span>

<span data-ttu-id="455a0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="455a0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="455a0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="455a0-127">Response</span></span>
<span data-ttu-id="455a0-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="455a0-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="455a0-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="455a0-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="455a0-130">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="455a0-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="455a0-131">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="455a0-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="455a0-132">Esta operação requer a permissão Presence. Read.</span><span class="sxs-lookup"><span data-stu-id="455a0-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="455a0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="455a0-133">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="455a0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="455a0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```
# <a name="c"></a>[<span data-ttu-id="455a0-135">C#</span><span class="sxs-lookup"><span data-stu-id="455a0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="455a0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="455a0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="455a0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="455a0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="455a0-138">Java</span><span class="sxs-lookup"><span data-stu-id="455a0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="455a0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="455a0-139">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="455a0-140">Exemplo 2: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="455a0-140">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="455a0-141">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="455a0-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="455a0-142">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="455a0-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="455a0-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="455a0-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="455a0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="455a0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="455a0-145">C#</span><span class="sxs-lookup"><span data-stu-id="455a0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="455a0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="455a0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="455a0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="455a0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="455a0-148">Java</span><span class="sxs-lookup"><span data-stu-id="455a0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="455a0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="455a0-149">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="455a0-150">Exemplo 3: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="455a0-150">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="455a0-151">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="455a0-151">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="455a0-152">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="455a0-152">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="455a0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="455a0-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="455a0-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="455a0-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="455a0-155">C#</span><span class="sxs-lookup"><span data-stu-id="455a0-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="455a0-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="455a0-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="455a0-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="455a0-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="455a0-158">Java</span><span class="sxs-lookup"><span data-stu-id="455a0-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="455a0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="455a0-159">Response</span></span>

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


