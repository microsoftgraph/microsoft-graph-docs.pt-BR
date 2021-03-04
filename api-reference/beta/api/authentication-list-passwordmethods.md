---
title: Listar senhaMethods
description: Recupere uma lista de objetos passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1184d095b5ea609dc7293948b69ac00673a07861
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438607"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="16b66-103">Listar senhaMethods</span><span class="sxs-lookup"><span data-stu-id="16b66-103">List passwordMethods</span></span>

<span data-ttu-id="16b66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16b66-105">Recupere uma lista de objetos [do método de autenticação de](../resources/passwordauthenticationmethod.md) senha.</span><span class="sxs-lookup"><span data-stu-id="16b66-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="16b66-106">Isso retornará exatamente um objeto, pois um usuário pode ter exatamente uma senha.</span><span class="sxs-lookup"><span data-stu-id="16b66-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="16b66-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16b66-107">Permissions</span></span>

<span data-ttu-id="16b66-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16b66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="16b66-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="16b66-110">Permissions acting on self</span></span>

|<span data-ttu-id="16b66-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16b66-111">Permission type</span></span>      | <span data-ttu-id="16b66-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16b66-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="16b66-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16b66-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="16b66-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b66-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="16b66-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16b66-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b66-116">Not supported.</span></span> |
| <span data-ttu-id="16b66-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16b66-117">Application</span></span>                            | <span data-ttu-id="16b66-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b66-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="16b66-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="16b66-119">Permissions acting on other users</span></span>

|<span data-ttu-id="16b66-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16b66-120">Permission type</span></span>      | <span data-ttu-id="16b66-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16b66-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="16b66-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16b66-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="16b66-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b66-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="16b66-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16b66-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b66-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b66-125">Not supported.</span></span> |
| <span data-ttu-id="16b66-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16b66-126">Application</span></span>                            | <span data-ttu-id="16b66-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b66-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="16b66-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="16b66-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="16b66-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="16b66-129">Global admin</span></span>
* <span data-ttu-id="16b66-130">Leitor global</span><span class="sxs-lookup"><span data-stu-id="16b66-130">Global reader</span></span>
* <span data-ttu-id="16b66-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="16b66-131">Privileged authentication admin</span></span>
* <span data-ttu-id="16b66-132">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="16b66-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="16b66-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16b66-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id | userPrincipalName}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16b66-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16b66-134">Optional query parameters</span></span>

<span data-ttu-id="16b66-135">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16b66-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16b66-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16b66-136">Request headers</span></span>

| <span data-ttu-id="16b66-137">Nome</span><span class="sxs-lookup"><span data-stu-id="16b66-137">Name</span></span>      |<span data-ttu-id="16b66-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="16b66-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16b66-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="16b66-139">Authorization</span></span> | <span data-ttu-id="16b66-140">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="16b66-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="16b66-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16b66-141">Request body</span></span>

<span data-ttu-id="16b66-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16b66-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b66-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b66-143">Response</span></span>

<span data-ttu-id="16b66-144">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16b66-144">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16b66-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16b66-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16b66-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16b66-146">Request</span></span>

<span data-ttu-id="16b66-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16b66-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16b66-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="16b66-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="16b66-149">C#</span><span class="sxs-lookup"><span data-stu-id="16b66-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16b66-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16b66-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16b66-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16b66-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16b66-152">Java</span><span class="sxs-lookup"><span data-stu-id="16b66-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordmethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16b66-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b66-153">Response</span></span>

<span data-ttu-id="16b66-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16b66-154">The following is an example of the response.</span></span>

> <span data-ttu-id="16b66-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16b66-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List passwordMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
