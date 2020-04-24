---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: Desabilitar a entrada do SMS para um telefone celular
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c887a78bc5bfe28112e608e6033bd2ed5064beba
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806459"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="b656b-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="b656b-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="b656b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b656b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b656b-105">Desabilite a entrada do SMS para um `mobile` número de telefone existente.</span><span class="sxs-lookup"><span data-stu-id="b656b-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="b656b-106">**Observação:** O número não estará mais disponível para entrada do SMS, que pode impedir o usuário de entrar.</span><span class="sxs-lookup"><span data-stu-id="b656b-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="b656b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b656b-107">Permissions</span></span>

<span data-ttu-id="b656b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b656b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b656b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b656b-110">Permission type</span></span>                        | <span data-ttu-id="b656b-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b656b-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="b656b-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b656b-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b656b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b656b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b656b-114">UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b656b-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="b656b-115">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b656b-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b656b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b656b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b656b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b656b-117">Not supported.</span></span> | <span data-ttu-id="b656b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b656b-118">Not supported.</span></span> |
| <span data-ttu-id="b656b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b656b-119">Application</span></span>                            | <span data-ttu-id="b656b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b656b-120">Not supported.</span></span> | <span data-ttu-id="b656b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b656b-121">Not supported.</span></span> |

<span data-ttu-id="b656b-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="b656b-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b656b-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b656b-123">Global admin</span></span>
* <span data-ttu-id="b656b-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="b656b-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b656b-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="b656b-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b656b-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b656b-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="b656b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b656b-127">Request headers</span></span>

| <span data-ttu-id="b656b-128">Nome</span><span class="sxs-lookup"><span data-stu-id="b656b-128">Name</span></span>          | <span data-ttu-id="b656b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b656b-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b656b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b656b-130">Authorization</span></span> | <span data-ttu-id="b656b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b656b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b656b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b656b-133">Request body</span></span>

<span data-ttu-id="b656b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b656b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b656b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b656b-135">Response</span></span>

<span data-ttu-id="b656b-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b656b-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b656b-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b656b-138">Examples</span></span>

<span data-ttu-id="b656b-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b656b-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b656b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b656b-140">Request</span></span>

<span data-ttu-id="b656b-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b656b-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b656b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b656b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="b656b-143">C#</span><span class="sxs-lookup"><span data-stu-id="b656b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b656b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b656b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b656b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b656b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b656b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b656b-146">Response</span></span>

<span data-ttu-id="b656b-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b656b-147">The following is an example of the response.</span></span>
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
