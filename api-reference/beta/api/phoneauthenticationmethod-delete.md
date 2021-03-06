---
title: Excluir phoneAuthenticationMethod
description: Exclua o método de autenticação de telefone de um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1abea19acd14c53d75e51783f8bd01fa8ed74d81
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516493"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="9b3ed-103">Excluir phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9b3ed-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="9b3ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b3ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b3ed-105">Excluir o método de autenticação [de telefone de um usuário.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="9b3ed-106">**Observação:** Isso remove o número de telefone do usuário e ele não poderá mais usar o número para autenticação, seja via SMS ou chamadas de voz.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="9b3ed-107">Lembre-se de que um usuário não pode ter `alternateMobile` um número sem um `mobile` número.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="9b3ed-108">Se você quiser remover um número de um usuário que também tenha um número, primeiro atualize o número para o novo número `mobile` `alternateMobile` e [](phoneauthenticationmethod-update.md) `mobile` exclua o `alternateMobile` número.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="9b3ed-109">Se o número de telefone for o método padrão de autenticação multifato do Azure (MFA), ele não poderá ser excluído.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="9b3ed-110">Fazer com que o usuário altere seu método de autenticação padrão e exclua o número.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b3ed-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b3ed-111">Permissions</span></span>

<span data-ttu-id="9b3ed-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b3ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9b3ed-114">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="9b3ed-114">Permissions acting on self</span></span>

|<span data-ttu-id="9b3ed-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b3ed-115">Permission type</span></span>      | <span data-ttu-id="9b3ed-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-116">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9b3ed-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b3ed-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b3ed-118">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9b3ed-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b3ed-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-120">Not supported.</span></span> |
| <span data-ttu-id="9b3ed-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b3ed-121">Application</span></span>                            | <span data-ttu-id="9b3ed-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-122">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9b3ed-123">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="9b3ed-123">Permissions acting on other users</span></span>

|<span data-ttu-id="9b3ed-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b3ed-124">Permission type</span></span>      | <span data-ttu-id="9b3ed-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-125">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9b3ed-126">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b3ed-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b3ed-127">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9b3ed-128">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b3ed-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-129">Not supported.</span></span> |
| <span data-ttu-id="9b3ed-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b3ed-130">Application</span></span>                            | <span data-ttu-id="9b3ed-131">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b3ed-131">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9b3ed-132">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9b3ed-132">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9b3ed-133">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9b3ed-133">Global admin</span></span>
* <span data-ttu-id="9b3ed-134">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="9b3ed-134">Privileged authentication admin</span></span>
* <span data-ttu-id="9b3ed-135">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="9b3ed-135">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9b3ed-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3ed-136">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9b3ed-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b3ed-137">Request headers</span></span>

| <span data-ttu-id="9b3ed-138">Nome</span><span class="sxs-lookup"><span data-stu-id="9b3ed-138">Name</span></span>          | <span data-ttu-id="9b3ed-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b3ed-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9b3ed-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b3ed-140">Authorization</span></span> | <span data-ttu-id="9b3ed-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b3ed-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b3ed-143">Request body</span></span>

<span data-ttu-id="9b3ed-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b3ed-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b3ed-145">Response</span></span>

<span data-ttu-id="9b3ed-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b3ed-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b3ed-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b3ed-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b3ed-149">Request</span></span>

<span data-ttu-id="9b3ed-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3ed-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3ed-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="9b3ed-152">C#</span><span class="sxs-lookup"><span data-stu-id="9b3ed-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3ed-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3ed-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3ed-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3ed-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b3ed-155">Java</span><span class="sxs-lookup"><span data-stu-id="9b3ed-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b3ed-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b3ed-156">Response</span></span>

<span data-ttu-id="9b3ed-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
