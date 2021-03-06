---
title: Listar senhaMethods
description: Recupere uma lista de objetos passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b0e03080bed41bc313e9cbe47f2e76b88999b66c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515475"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="07c5a-103">Listar senhaMethods</span><span class="sxs-lookup"><span data-stu-id="07c5a-103">List passwordMethods</span></span>

<span data-ttu-id="07c5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c5a-105">Recupere uma lista de objetos [do método de autenticação de](../resources/passwordauthenticationmethod.md) senha.</span><span class="sxs-lookup"><span data-stu-id="07c5a-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="07c5a-106">Isso retornará exatamente um objeto, pois um usuário pode ter exatamente uma senha.</span><span class="sxs-lookup"><span data-stu-id="07c5a-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c5a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="07c5a-107">Permissions</span></span>

<span data-ttu-id="07c5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="07c5a-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="07c5a-110">Permissions acting on self</span></span>

|<span data-ttu-id="07c5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07c5a-111">Permission type</span></span>      | <span data-ttu-id="07c5a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07c5a-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="07c5a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07c5a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="07c5a-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07c5a-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="07c5a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07c5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c5a-116">Not supported.</span></span> |
| <span data-ttu-id="07c5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07c5a-117">Application</span></span>                            | <span data-ttu-id="07c5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c5a-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="07c5a-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="07c5a-119">Permissions acting on other users</span></span>

|<span data-ttu-id="07c5a-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07c5a-120">Permission type</span></span>      | <span data-ttu-id="07c5a-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07c5a-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="07c5a-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07c5a-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="07c5a-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c5a-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="07c5a-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07c5a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c5a-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c5a-125">Not supported.</span></span> |
| <span data-ttu-id="07c5a-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07c5a-126">Application</span></span>                            | <span data-ttu-id="07c5a-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c5a-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="07c5a-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="07c5a-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="07c5a-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="07c5a-129">Global admin</span></span>
* <span data-ttu-id="07c5a-130">Leitor global</span><span class="sxs-lookup"><span data-stu-id="07c5a-130">Global reader</span></span>
* <span data-ttu-id="07c5a-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="07c5a-131">Privileged authentication admin</span></span>
* <span data-ttu-id="07c5a-132">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="07c5a-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="07c5a-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07c5a-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id | userPrincipalName}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07c5a-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07c5a-134">Optional query parameters</span></span>

<span data-ttu-id="07c5a-135">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07c5a-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07c5a-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07c5a-136">Request headers</span></span>

| <span data-ttu-id="07c5a-137">Nome</span><span class="sxs-lookup"><span data-stu-id="07c5a-137">Name</span></span>      |<span data-ttu-id="07c5a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="07c5a-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07c5a-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="07c5a-139">Authorization</span></span> | <span data-ttu-id="07c5a-140">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="07c5a-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c5a-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07c5a-141">Request body</span></span>

<span data-ttu-id="07c5a-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07c5a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07c5a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c5a-143">Response</span></span>

<span data-ttu-id="07c5a-144">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07c5a-144">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07c5a-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="07c5a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07c5a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07c5a-146">Request</span></span>

<span data-ttu-id="07c5a-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07c5a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07c5a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="07c5a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="07c5a-149">C#</span><span class="sxs-lookup"><span data-stu-id="07c5a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07c5a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07c5a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07c5a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07c5a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07c5a-152">Java</span><span class="sxs-lookup"><span data-stu-id="07c5a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordmethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07c5a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c5a-153">Response</span></span>

<span data-ttu-id="07c5a-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07c5a-154">The following is an example of the response.</span></span>

> <span data-ttu-id="07c5a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07c5a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
