---
title: Atualizar b2cAuthenticationMethodsPolicy
description: Atualize as propriedades de um objeto b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aed20c26bab07cb6778b80d10e3becf33e998409
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961265"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="fd9c3-103">Atualizar b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="fd9c3-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="fd9c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd9c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd9c3-105">Atualize as propriedades de um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd9c3-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd9c3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd9c3-106">Permissions</span></span>

<span data-ttu-id="fd9c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd9c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd9c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd9c3-109">Permission type</span></span>                        | <span data-ttu-id="fd9c3-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd9c3-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="fd9c3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd9c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd9c3-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fd9c3-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="fd9c3-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="fd9c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd9c3-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fd9c3-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="fd9c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd9c3-115">Application</span></span>                            | <span data-ttu-id="fd9c3-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fd9c3-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd9c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd9c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="fd9c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd9c3-118">Request headers</span></span>

|<span data-ttu-id="fd9c3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fd9c3-119">Name</span></span>|<span data-ttu-id="fd9c3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd9c3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fd9c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd9c3-121">Authorization</span></span>|<span data-ttu-id="fd9c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd9c3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd9c3-124">Content-Type</span></span>|<span data-ttu-id="fd9c3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd9c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd9c3-127">Request body</span></span>

<span data-ttu-id="fd9c3-128">No corpo da solicitação, forneça uma representação JSON do objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd9c3-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="fd9c3-129">A tabela a seguir mostra as propriedades obrigatórias ao atualizar [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd9c3-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="fd9c3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd9c3-130">Property</span></span>     | <span data-ttu-id="fd9c3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd9c3-131">Type</span></span>        | <span data-ttu-id="fd9c3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd9c3-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd9c3-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="fd9c3-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="fd9c3-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd9c3-134">Boolean</span></span>|<span data-ttu-id="fd9c3-135">O administrador de locatário pode configurar contas locais usando o email se o método de autenticação de email e senha estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="fd9c3-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="fd9c3-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="fd9c3-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd9c3-137">Boolean</span></span>|<span data-ttu-id="fd9c3-138">O administrador de locatários pode configurar contas locais usando o nome de usuário se o método de autenticação do nome de usuário e senha estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-138">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="fd9c3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd9c3-139">Response</span></span>

<span data-ttu-id="fd9c3-140">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd9c3-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fd9c3-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd9c3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd9c3-142">Request</span></span>

<span data-ttu-id="fd9c3-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fd9c3-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd9c3-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="fd9c3-145">C#</span><span class="sxs-lookup"><span data-stu-id="fd9c3-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd9c3-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd9c3-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd9c3-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd9c3-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd9c3-148">Java</span><span class="sxs-lookup"><span data-stu-id="fd9c3-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fd9c3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd9c3-149">Response</span></span>

<span data-ttu-id="fd9c3-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fd9c3-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cauthenticationmethodspolicy"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update b2cauthenticationmethodspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
