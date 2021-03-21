---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: Habilitar a assinatura SMS para um telefone celular.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: def7c4409ea38adf1764a7b3f1adf1d9280b992a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957308"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="7aa64-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="7aa64-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="7aa64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa64-105">Habilitar a login sms para um número `mobile` de telefone existente.</span><span class="sxs-lookup"><span data-stu-id="7aa64-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="7aa64-106">Para ser habilitado com êxito:</span><span class="sxs-lookup"><span data-stu-id="7aa64-106">To be successfully enabled:</span></span>

* <span data-ttu-id="7aa64-107">O telefone deve ter `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="7aa64-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="7aa64-108">O telefone deve ser exclusivo no sistema de login SMS (ninguém mais também pode usar esse número).</span><span class="sxs-lookup"><span data-stu-id="7aa64-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="7aa64-109">O usuário deve estar habilitado para entrar SMS na política [de métodos de](/azure/active-directory/authentication/concept-authentication-methods) autenticação.</span><span class="sxs-lookup"><span data-stu-id="7aa64-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa64-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aa64-110">Permissions</span></span>

<span data-ttu-id="7aa64-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="7aa64-113">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="7aa64-113">Permissions acting on self</span></span>

|<span data-ttu-id="7aa64-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aa64-114">Permission type</span></span>      | <span data-ttu-id="7aa64-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7aa64-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="7aa64-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aa64-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aa64-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aa64-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="7aa64-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aa64-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa64-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aa64-119">Not supported.</span></span> |
| <span data-ttu-id="7aa64-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aa64-120">Application</span></span>                            | <span data-ttu-id="7aa64-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aa64-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="7aa64-122">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="7aa64-122">Permissions acting on other users</span></span>

|<span data-ttu-id="7aa64-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aa64-123">Permission type</span></span>      | <span data-ttu-id="7aa64-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7aa64-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="7aa64-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aa64-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aa64-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa64-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="7aa64-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aa64-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa64-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aa64-128">Not supported.</span></span> |
| <span data-ttu-id="7aa64-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aa64-129">Application</span></span>                            | <span data-ttu-id="7aa64-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa64-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="7aa64-131">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="7aa64-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="7aa64-132">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7aa64-132">Global admin</span></span>
* <span data-ttu-id="7aa64-133">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="7aa64-133">Privileged authentication admin</span></span>
* <span data-ttu-id="7aa64-134">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="7aa64-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="7aa64-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aa64-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```
<span data-ttu-id="7aa64-136">O valor de `id` para `mobile` o phoneType é `3179e48a-750b-4051-897c-87b9720928f7` .</span><span class="sxs-lookup"><span data-stu-id="7aa64-136">The value of `id` for the `mobile` phoneType is `3179e48a-750b-4051-897c-87b9720928f7`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aa64-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa64-137">Request headers</span></span>

| <span data-ttu-id="7aa64-138">Nome</span><span class="sxs-lookup"><span data-stu-id="7aa64-138">Name</span></span>          | <span data-ttu-id="7aa64-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa64-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7aa64-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aa64-140">Authorization</span></span> | <span data-ttu-id="7aa64-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aa64-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aa64-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa64-143">Request body</span></span>

<span data-ttu-id="7aa64-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7aa64-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aa64-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa64-145">Response</span></span>

<span data-ttu-id="7aa64-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa64-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7aa64-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7aa64-148">Examples</span></span>

<span data-ttu-id="7aa64-149">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7aa64-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7aa64-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa64-150">Request</span></span>

<span data-ttu-id="7aa64-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aa64-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7aa64-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aa64-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="7aa64-153">C#</span><span class="sxs-lookup"><span data-stu-id="7aa64-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7aa64-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aa64-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7aa64-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aa64-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7aa64-156">Java</span><span class="sxs-lookup"><span data-stu-id="7aa64-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7aa64-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa64-157">Response</span></span>

<span data-ttu-id="7aa64-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa64-158">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
