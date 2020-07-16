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
# <a name="riskyuser-dismiss"></a><span data-ttu-id="55362-103">riskyUser: fechar</span><span class="sxs-lookup"><span data-stu-id="55362-103">riskyUser: dismiss</span></span>

<span data-ttu-id="55362-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55362-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="55362-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="55362-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="55362-106">Descarte o risco de um ou mais objetos [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="55362-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="55362-107">Esta ação define o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="55362-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="55362-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="55362-108">Permissions</span></span>
<span data-ttu-id="55362-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55362-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55362-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55362-111">Permission type</span></span>      | <span data-ttu-id="55362-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55362-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55362-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55362-113">Delegated (work or school account)</span></span> | <span data-ttu-id="55362-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55362-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="55362-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55362-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55362-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55362-116">Not supported.</span></span>    |
|<span data-ttu-id="55362-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55362-117">Application</span></span> | <span data-ttu-id="55362-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55362-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55362-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55362-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="55362-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55362-120">Request headers</span></span>
| <span data-ttu-id="55362-121">Nome</span><span class="sxs-lookup"><span data-stu-id="55362-121">Name</span></span>      |<span data-ttu-id="55362-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="55362-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55362-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55362-123">Authorization</span></span>  | <span data-ttu-id="55362-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55362-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55362-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55362-126">Request body</span></span>
<span data-ttu-id="55362-127">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55362-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="55362-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="55362-128">Response</span></span>

<span data-ttu-id="55362-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55362-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="55362-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55362-131">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="55362-132">Exemplo 1: ignorar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="55362-132">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="55362-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55362-133">Request</span></span>
<span data-ttu-id="55362-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55362-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55362-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="55362-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="55362-136">C#</span><span class="sxs-lookup"><span data-stu-id="55362-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55362-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55362-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55362-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55362-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55362-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="55362-139">Response</span></span>
<span data-ttu-id="55362-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55362-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="55362-141">Exemplo 2: descartar um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="55362-141">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="55362-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55362-142">Request</span></span>
<span data-ttu-id="55362-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55362-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55362-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="55362-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="55362-145">C#</span><span class="sxs-lookup"><span data-stu-id="55362-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55362-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55362-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55362-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55362-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55362-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="55362-148">Response</span></span>
<span data-ttu-id="55362-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55362-149">Here is an example of the response.</span></span>
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
