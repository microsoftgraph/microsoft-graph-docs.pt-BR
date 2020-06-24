---
title: Ignorar riskyUser
description: Descartar o risco de um objeto riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 3a549ca4b50d1a0e873a905a6312e30d6bf1e838
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863513"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="095de-103">riskyUser: fechar</span><span class="sxs-lookup"><span data-stu-id="095de-103">riskyUser: dismiss</span></span>

<span data-ttu-id="095de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="095de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="095de-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="095de-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="095de-106">Descarte o risco de um ou mais objetos [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="095de-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="095de-107">Esta ação define o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="095de-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="095de-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="095de-108">Permissions</span></span>
<span data-ttu-id="095de-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="095de-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="095de-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="095de-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="095de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="095de-111">Permission type</span></span>      | <span data-ttu-id="095de-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="095de-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="095de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="095de-113">Delegated (work or school account)</span></span> | <span data-ttu-id="095de-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095de-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="095de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="095de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="095de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="095de-116">Not supported.</span></span>    |
|<span data-ttu-id="095de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="095de-117">Application</span></span> | <span data-ttu-id="095de-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095de-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="095de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="095de-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="095de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="095de-120">Request headers</span></span>
| <span data-ttu-id="095de-121">Nome</span><span class="sxs-lookup"><span data-stu-id="095de-121">Name</span></span>      |<span data-ttu-id="095de-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="095de-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="095de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="095de-123">Authorization</span></span>  | <span data-ttu-id="095de-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="095de-124">Bearer {token}.</span></span> <span data-ttu-id="095de-125">Required.</span><span class="sxs-lookup"><span data-stu-id="095de-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="095de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="095de-126">Request body</span></span>
<span data-ttu-id="095de-127">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="095de-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="095de-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="095de-128">Response</span></span>

<span data-ttu-id="095de-129">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="095de-129">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="095de-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="095de-130">It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="095de-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="095de-131">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="095de-132">Exemplo 1: ignorar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="095de-132">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="095de-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="095de-133">Request</span></span>
<span data-ttu-id="095de-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="095de-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="095de-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="095de-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="095de-136">C#</span><span class="sxs-lookup"><span data-stu-id="095de-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="095de-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="095de-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="095de-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="095de-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="095de-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="095de-139">Response</span></span>
<span data-ttu-id="095de-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="095de-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="095de-141">Exemplo 2: descartar um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="095de-141">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="095de-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="095de-142">Request</span></span>
<span data-ttu-id="095de-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="095de-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="095de-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="095de-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="095de-145">C#</span><span class="sxs-lookup"><span data-stu-id="095de-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="095de-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="095de-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="095de-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="095de-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="095de-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="095de-148">Response</span></span>
<span data-ttu-id="095de-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="095de-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
