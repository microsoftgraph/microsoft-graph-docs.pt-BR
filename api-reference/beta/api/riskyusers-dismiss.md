---
title: Descartar riskyUser
description: Descartar o risco de um objeto riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 47b749e1ac5d782d96210b493ed1451db19184c7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761483"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="5a149-103">riskyUser: dismiss</span><span class="sxs-lookup"><span data-stu-id="5a149-103">riskyUser: dismiss</span></span>

<span data-ttu-id="5a149-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a149-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="5a149-105">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5a149-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="5a149-106">Descartar o risco de um ou mais [objetos riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5a149-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="5a149-107">Essa ação define o nível de risco do usuário direcionado como nenhum.</span><span class="sxs-lookup"><span data-stu-id="5a149-107">This action sets the targeted user's risk level to none.</span></span> <span data-ttu-id="5a149-108">A contagem máxima de usuários a ser descartada em uma chamada é 60.</span><span class="sxs-lookup"><span data-stu-id="5a149-108">The maximum count of users to dismiss in one call is 60.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a149-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a149-109">Permissions</span></span>
<span data-ttu-id="5a149-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a149-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a149-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a149-112">Permission type</span></span>      | <span data-ttu-id="5a149-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a149-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a149-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a149-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5a149-115">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a149-115">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a149-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a149-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a149-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a149-117">Not supported.</span></span>    |
|<span data-ttu-id="5a149-118">Application</span><span class="sxs-lookup"><span data-stu-id="5a149-118">Application</span></span> | <span data-ttu-id="5a149-119">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a149-119">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a149-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a149-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="5a149-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a149-121">Request headers</span></span>
| <span data-ttu-id="5a149-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5a149-122">Name</span></span>      |<span data-ttu-id="5a149-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a149-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a149-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a149-124">Authorization</span></span>  | <span data-ttu-id="5a149-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a149-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a149-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a149-127">Request body</span></span>
<span data-ttu-id="5a149-128">Especifique os userIds a descartar no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a149-128">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="5a149-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a149-129">Response</span></span>

<span data-ttu-id="5a149-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a149-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="5a149-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5a149-132">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="5a149-133">Exemplo 1: descartar usuários arriscados</span><span class="sxs-lookup"><span data-stu-id="5a149-133">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="5a149-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a149-134">Request</span></span>
<span data-ttu-id="5a149-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a149-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a149-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a149-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a149-137">C#</span><span class="sxs-lookup"><span data-stu-id="5a149-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a149-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a149-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a149-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a149-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a149-140">Java</span><span class="sxs-lookup"><span data-stu-id="5a149-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5a149-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a149-141">Response</span></span>
<span data-ttu-id="5a149-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a149-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="5a149-143">Exemplo 2: descartar um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="5a149-143">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="5a149-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a149-144">Request</span></span>
<span data-ttu-id="5a149-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a149-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a149-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a149-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a149-147">C#</span><span class="sxs-lookup"><span data-stu-id="5a149-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a149-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a149-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a149-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a149-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a149-150">Java</span><span class="sxs-lookup"><span data-stu-id="5a149-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5a149-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a149-151">Response</span></span>
<span data-ttu-id="5a149-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a149-152">Here is an example of the response.</span></span>
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


