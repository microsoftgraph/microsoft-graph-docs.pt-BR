---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: d9f3b141144654e21c47c523c46a3329865c7031
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970937"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="0fe4b-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="0fe4b-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="0fe4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fe4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="0fe4b-105">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="0fe4b-106">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="0fe4b-107">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe4b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fe4b-108">Permissions</span></span>
<span data-ttu-id="0fe4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fe4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fe4b-111">Permission type</span></span>      | <span data-ttu-id="0fe4b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fe4b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fe4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fe4b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0fe4b-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe4b-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fe4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fe4b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fe4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-116">Not supported.</span></span>    |
|<span data-ttu-id="0fe4b-117">Application</span><span class="sxs-lookup"><span data-stu-id="0fe4b-117">Application</span></span> | <span data-ttu-id="0fe4b-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe4b-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe4b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="0fe4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe4b-120">Request headers</span></span>
| <span data-ttu-id="0fe4b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0fe4b-121">Name</span></span>      |<span data-ttu-id="0fe4b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fe4b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0fe4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fe4b-123">Authorization</span></span>  | <span data-ttu-id="0fe4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fe4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe4b-126">Request body</span></span>
<span data-ttu-id="0fe4b-127">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="0fe4b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe4b-128">Response</span></span>

<span data-ttu-id="0fe4b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="0fe4b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0fe4b-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="0fe4b-132">Exemplo 1: confirmar os usuários como comprometidos</span><span class="sxs-lookup"><span data-stu-id="0fe4b-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="0fe4b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe4b-133">Request</span></span>
<span data-ttu-id="0fe4b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fe4b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe4b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="0fe4b-136">C#</span><span class="sxs-lookup"><span data-stu-id="0fe4b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fe4b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fe4b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fe4b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fe4b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fe4b-139">Java</span><span class="sxs-lookup"><span data-stu-id="0fe4b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0fe4b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe4b-140">Response</span></span>
<span data-ttu-id="0fe4b-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="0fe4b-142">Exemplo 2: confirmar um usuário como comprometido</span><span class="sxs-lookup"><span data-stu-id="0fe4b-142">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="0fe4b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe4b-143">Request</span></span>
<span data-ttu-id="0fe4b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fe4b-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe4b-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="0fe4b-146">C#</span><span class="sxs-lookup"><span data-stu-id="0fe4b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fe4b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fe4b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fe4b-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fe4b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fe4b-149">Java</span><span class="sxs-lookup"><span data-stu-id="0fe4b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0fe4b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe4b-150">Response</span></span>
<span data-ttu-id="0fe4b-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe4b-151">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


