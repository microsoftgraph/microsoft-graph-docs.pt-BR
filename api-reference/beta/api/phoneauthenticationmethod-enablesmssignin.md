---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: Habilita SMS entrar para um telefone celular.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1452d3e3e1c93def07dce3b6ee78a996c374ae0c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786460"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="86f1b-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="86f1b-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="86f1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86f1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86f1b-105">Habilita SMS entrar para um número de `mobile` telefone existente.</span><span class="sxs-lookup"><span data-stu-id="86f1b-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="86f1b-106">Para ser habilitado com êxito:</span><span class="sxs-lookup"><span data-stu-id="86f1b-106">To be successfully enabled:</span></span>

* <span data-ttu-id="86f1b-107">O telefone deve ter `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="86f1b-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="86f1b-108">O telefone deve ser exclusivo no sistema de SMS de login (ninguém mais também pode usar esse número).</span><span class="sxs-lookup"><span data-stu-id="86f1b-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="86f1b-109">O usuário deve estar habilitado para SMS entrar na política [de métodos de autenticação.](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="86f1b-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="86f1b-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="86f1b-110">Permissions</span></span>

<span data-ttu-id="86f1b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86f1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="86f1b-113">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="86f1b-113">Permissions acting on self</span></span>

|<span data-ttu-id="86f1b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86f1b-114">Permission type</span></span>      | <span data-ttu-id="86f1b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86f1b-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="86f1b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86f1b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="86f1b-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86f1b-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="86f1b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86f1b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86f1b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86f1b-119">Not supported.</span></span> |
| <span data-ttu-id="86f1b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86f1b-120">Application</span></span>                            | <span data-ttu-id="86f1b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86f1b-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="86f1b-122">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="86f1b-122">Permissions acting on other users</span></span>

|<span data-ttu-id="86f1b-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86f1b-123">Permission type</span></span>      | <span data-ttu-id="86f1b-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86f1b-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="86f1b-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86f1b-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="86f1b-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86f1b-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="86f1b-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86f1b-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86f1b-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86f1b-128">Not supported.</span></span> |
| <span data-ttu-id="86f1b-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86f1b-129">Application</span></span>                            | <span data-ttu-id="86f1b-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86f1b-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="86f1b-131">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="86f1b-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="86f1b-132">Administrador global</span><span class="sxs-lookup"><span data-stu-id="86f1b-132">Global admin</span></span>
* <span data-ttu-id="86f1b-133">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="86f1b-133">Privileged authentication admin</span></span>
* <span data-ttu-id="86f1b-134">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="86f1b-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="86f1b-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86f1b-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```
<span data-ttu-id="86f1b-136">O valor de `id` para `mobile` o phoneType é `3179e48a-750b-4051-897c-87b9720928f7` .</span><span class="sxs-lookup"><span data-stu-id="86f1b-136">The value of `id` for the `mobile` phoneType is `3179e48a-750b-4051-897c-87b9720928f7`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86f1b-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86f1b-137">Request headers</span></span>

| <span data-ttu-id="86f1b-138">Nome</span><span class="sxs-lookup"><span data-stu-id="86f1b-138">Name</span></span>          | <span data-ttu-id="86f1b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="86f1b-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="86f1b-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="86f1b-140">Authorization</span></span> | <span data-ttu-id="86f1b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86f1b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86f1b-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86f1b-143">Request body</span></span>

<span data-ttu-id="86f1b-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86f1b-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86f1b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="86f1b-145">Response</span></span>

<span data-ttu-id="86f1b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86f1b-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86f1b-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="86f1b-148">Examples</span></span>

<span data-ttu-id="86f1b-149">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="86f1b-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="86f1b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86f1b-150">Request</span></span>

<span data-ttu-id="86f1b-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86f1b-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86f1b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="86f1b-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="86f1b-153">C#</span><span class="sxs-lookup"><span data-stu-id="86f1b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86f1b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86f1b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86f1b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86f1b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86f1b-156">Java</span><span class="sxs-lookup"><span data-stu-id="86f1b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86f1b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="86f1b-157">Response</span></span>

<span data-ttu-id="86f1b-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86f1b-158">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: enableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
