---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: Desabilitar a entrada do SMS para um telefone celular
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f2fcb5011640881ca53fd3c642172e19402359af
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461031"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="c81e0-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="c81e0-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="c81e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c81e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c81e0-105">Desabilite a entrada do SMS para um `mobile` número de telefone existente.</span><span class="sxs-lookup"><span data-stu-id="c81e0-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="c81e0-106">**Observação:** O número não estará mais disponível para entrada do SMS, que pode impedir o usuário de entrar.</span><span class="sxs-lookup"><span data-stu-id="c81e0-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="c81e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c81e0-107">Permissions</span></span>

<span data-ttu-id="c81e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c81e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c81e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c81e0-110">Permission type</span></span>                        | <span data-ttu-id="c81e0-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c81e0-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="c81e0-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c81e0-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="c81e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c81e0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c81e0-114">UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c81e0-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="c81e0-115">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c81e0-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c81e0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c81e0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c81e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c81e0-117">Not supported.</span></span> | <span data-ttu-id="c81e0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c81e0-118">Not supported.</span></span> |
| <span data-ttu-id="c81e0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c81e0-119">Application</span></span>                            | <span data-ttu-id="c81e0-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c81e0-120">Not supported.</span></span> | <span data-ttu-id="c81e0-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c81e0-121">Not supported.</span></span> |

<span data-ttu-id="c81e0-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="c81e0-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c81e0-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c81e0-123">Global admin</span></span>
* <span data-ttu-id="c81e0-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c81e0-124">Privileged authentication admin</span></span>
* <span data-ttu-id="c81e0-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="c81e0-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c81e0-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c81e0-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="c81e0-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c81e0-127">Request headers</span></span>

| <span data-ttu-id="c81e0-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c81e0-128">Name</span></span>          | <span data-ttu-id="c81e0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c81e0-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c81e0-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c81e0-130">Authorization</span></span> | <span data-ttu-id="c81e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c81e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c81e0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c81e0-133">Request body</span></span>

<span data-ttu-id="c81e0-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c81e0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c81e0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c81e0-135">Response</span></span>

<span data-ttu-id="c81e0-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c81e0-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c81e0-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c81e0-138">Examples</span></span>

<span data-ttu-id="c81e0-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c81e0-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c81e0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c81e0-140">Request</span></span>

<span data-ttu-id="c81e0-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c81e0-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c81e0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c81e0-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="c81e0-143">C#</span><span class="sxs-lookup"><span data-stu-id="c81e0-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c81e0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c81e0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c81e0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c81e0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c81e0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c81e0-146">Response</span></span>

<span data-ttu-id="c81e0-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c81e0-147">The following is an example of the response.</span></span>
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
