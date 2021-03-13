---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 06de240619f121671b6fea8883bca0d3fa19e38a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760943"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="64773-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="64773-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="64773-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="64773-105">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="64773-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="64773-106">Confirme um ou mais [objetos riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="64773-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="64773-107">Essa ação define o nível de risco do usuário direcionado como alto.</span><span class="sxs-lookup"><span data-stu-id="64773-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="64773-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="64773-108">Permissions</span></span>
<span data-ttu-id="64773-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64773-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64773-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64773-111">Permission type</span></span>      | <span data-ttu-id="64773-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64773-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64773-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64773-113">Delegated (work or school account)</span></span> | <span data-ttu-id="64773-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64773-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="64773-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64773-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64773-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64773-116">Not supported.</span></span>    |
|<span data-ttu-id="64773-117">Application</span><span class="sxs-lookup"><span data-stu-id="64773-117">Application</span></span> | <span data-ttu-id="64773-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64773-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64773-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64773-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="64773-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64773-120">Request headers</span></span>
| <span data-ttu-id="64773-121">Nome</span><span class="sxs-lookup"><span data-stu-id="64773-121">Name</span></span>      |<span data-ttu-id="64773-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="64773-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64773-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64773-123">Authorization</span></span>  | <span data-ttu-id="64773-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64773-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64773-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64773-126">Request body</span></span>
<span data-ttu-id="64773-127">Especifique as IDs de usuário arriscadas para descartar no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64773-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="64773-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="64773-128">Response</span></span>

<span data-ttu-id="64773-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64773-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="64773-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64773-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="64773-132">Exemplo 1: Confirmar usuários como comprometidos</span><span class="sxs-lookup"><span data-stu-id="64773-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="64773-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64773-133">Request</span></span>
<span data-ttu-id="64773-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64773-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64773-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="64773-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="64773-136">C#</span><span class="sxs-lookup"><span data-stu-id="64773-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64773-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64773-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64773-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64773-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64773-139">Java</span><span class="sxs-lookup"><span data-stu-id="64773-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="64773-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="64773-140">Response</span></span>
<span data-ttu-id="64773-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64773-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="64773-142">Exemplo 2: Confirmar um usuário como comprometido</span><span class="sxs-lookup"><span data-stu-id="64773-142">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="64773-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64773-143">Request</span></span>
<span data-ttu-id="64773-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64773-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64773-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="64773-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="64773-146">C#</span><span class="sxs-lookup"><span data-stu-id="64773-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64773-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64773-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64773-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64773-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64773-149">Java</span><span class="sxs-lookup"><span data-stu-id="64773-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="64773-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="64773-150">Response</span></span>
<span data-ttu-id="64773-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64773-151">Here is an example of the response.</span></span>
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


