---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: Desabilitar a login do SMS para um telefone celular
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 235257c4df9c24dec33aad15e11b2318e0fb8e30
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447682"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="55124-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="55124-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="55124-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55124-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55124-105">Desabilite a login do SMS para um número `mobile` de telefone existente.</span><span class="sxs-lookup"><span data-stu-id="55124-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="55124-106">**Observação:** O número não estará mais disponível para a assinatura sms, o que pode impedir que o usuário entre.</span><span class="sxs-lookup"><span data-stu-id="55124-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="55124-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="55124-107">Permissions</span></span>

<span data-ttu-id="55124-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="55124-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="55124-110">Permissions acting on self</span></span>

|<span data-ttu-id="55124-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55124-111">Permission type</span></span>      | <span data-ttu-id="55124-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55124-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="55124-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55124-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="55124-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55124-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="55124-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55124-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55124-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55124-116">Not supported.</span></span> |
| <span data-ttu-id="55124-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55124-117">Application</span></span>                            | <span data-ttu-id="55124-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55124-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="55124-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="55124-119">Permissions acting on other users</span></span>

|<span data-ttu-id="55124-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55124-120">Permission type</span></span>      | <span data-ttu-id="55124-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55124-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="55124-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55124-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="55124-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55124-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="55124-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55124-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55124-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55124-125">Not supported.</span></span> |
| <span data-ttu-id="55124-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55124-126">Application</span></span>                            | <span data-ttu-id="55124-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55124-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="55124-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="55124-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="55124-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="55124-129">Global admin</span></span>
* <span data-ttu-id="55124-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="55124-130">Privileged authentication admin</span></span>
* <span data-ttu-id="55124-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="55124-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="55124-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55124-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="55124-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55124-133">Request headers</span></span>

| <span data-ttu-id="55124-134">Nome</span><span class="sxs-lookup"><span data-stu-id="55124-134">Name</span></span>          | <span data-ttu-id="55124-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="55124-135">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="55124-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="55124-136">Authorization</span></span> | <span data-ttu-id="55124-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55124-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55124-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55124-139">Request body</span></span>

<span data-ttu-id="55124-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55124-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55124-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="55124-141">Response</span></span>

<span data-ttu-id="55124-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55124-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55124-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55124-144">Examples</span></span>

<span data-ttu-id="55124-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="55124-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="55124-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55124-146">Request</span></span>

<span data-ttu-id="55124-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55124-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55124-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="55124-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="55124-149">C#</span><span class="sxs-lookup"><span data-stu-id="55124-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55124-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55124-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55124-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55124-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55124-152">Java</span><span class="sxs-lookup"><span data-stu-id="55124-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55124-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="55124-153">Response</span></span>

<span data-ttu-id="55124-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55124-154">The following is an example of the response.</span></span>
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
  "description": "phoneAuthenticationMethod: disableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
