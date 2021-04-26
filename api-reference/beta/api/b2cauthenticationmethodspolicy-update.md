---
title: Atualizar b2cAuthenticationMethodsPolicy
description: Atualize as propriedades de um objeto b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f2da149c32e10c0871decf1f8be96144b66b173a
ms.sourcegitcommit: 92f545d2d9af13ac7aff9932eb265f136d089f79
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51996119"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="3929d-103">Atualizar b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="3929d-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="3929d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3929d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3929d-105">Atualize as propriedades de um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3929d-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3929d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3929d-106">Permissions</span></span>

<span data-ttu-id="3929d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3929d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3929d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3929d-109">Permission type</span></span>                        | <span data-ttu-id="3929d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3929d-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="3929d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3929d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3929d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3929d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="3929d-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="3929d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3929d-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3929d-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="3929d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3929d-115">Application</span></span>                            | <span data-ttu-id="3929d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3929d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="3929d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3929d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="3929d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3929d-118">Request headers</span></span>

|<span data-ttu-id="3929d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3929d-119">Name</span></span>|<span data-ttu-id="3929d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3929d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3929d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3929d-121">Authorization</span></span>|<span data-ttu-id="3929d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3929d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3929d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3929d-124">Content-Type</span></span>|<span data-ttu-id="3929d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3929d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3929d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3929d-127">Request body</span></span>

<span data-ttu-id="3929d-128">No corpo da solicitação, forneça uma representação JSON do objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3929d-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="3929d-129">A tabela a seguir mostra as propriedades obrigatórias ao atualizar [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3929d-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="3929d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3929d-130">Property</span></span>     | <span data-ttu-id="3929d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3929d-131">Type</span></span>        | <span data-ttu-id="3929d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3929d-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3929d-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="3929d-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="3929d-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="3929d-134">Boolean</span></span>|<span data-ttu-id="3929d-135">O administrador de locatário pode configurar contas locais usando o email se o método de autenticação de email e senha estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="3929d-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="3929d-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="3929d-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="3929d-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="3929d-137">Boolean</span></span>|<span data-ttu-id="3929d-138">O administrador de locatários pode configurar contas locais usando o nome de usuário se o método de autenticação do nome de usuário e senha estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="3929d-138">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|
|<span data-ttu-id="3929d-139">isPhoneOneTimePasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="3929d-139">isPhoneOneTimePasswordAuthenticationEnabled</span></span>|<span data-ttu-id="3929d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3929d-140">Boolean</span></span>|<span data-ttu-id="3929d-141">O administrador de locatários poderá configurar contas locais usando o número de telefone se o número de telefone e o método de autenticação de senha única estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="3929d-141">The tenant admin can configure local accounts using phone number if the phone number and one-time password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="3929d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3929d-142">Response</span></span>

<span data-ttu-id="3929d-143">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="3929d-143">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3929d-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3929d-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3929d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3929d-145">Request</span></span>

<span data-ttu-id="3929d-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3929d-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3929d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3929d-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true,
    "isPhoneOneTimePasswordAuthenticationEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="3929d-148">C#</span><span class="sxs-lookup"><span data-stu-id="3929d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3929d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3929d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3929d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3929d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3929d-151">Java</span><span class="sxs-lookup"><span data-stu-id="3929d-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3929d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="3929d-152">Response</span></span>

<span data-ttu-id="3929d-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3929d-153">The following is an example of the response.</span></span>

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
