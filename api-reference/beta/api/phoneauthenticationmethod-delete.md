---
title: Excluir phoneAuthenticationMethod
description: Exclua o método de autenticação de telefone de um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bbd08b9da7a75c471e90b9846e3aaa2c1a503879
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957482"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="43a2a-103">Excluir phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="43a2a-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="43a2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43a2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43a2a-105">Excluir o método de autenticação [de telefone de um usuário.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="43a2a-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="43a2a-106">**Observação:** Isso remove o número de telefone do usuário e ele não poderá mais usar o número para autenticação, seja via SMS ou chamadas de voz.</span><span class="sxs-lookup"><span data-stu-id="43a2a-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="43a2a-107">Lembre-se de que um usuário não pode ter `alternateMobile` um número sem um `mobile` número.</span><span class="sxs-lookup"><span data-stu-id="43a2a-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="43a2a-108">Se você quiser remover um número de um usuário que também tenha um número, primeiro atualize o número para o novo número `mobile` `alternateMobile` e [](phoneauthenticationmethod-update.md) `mobile` exclua o `alternateMobile` número.</span><span class="sxs-lookup"><span data-stu-id="43a2a-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="43a2a-109">Se o número de telefone for o método padrão de autenticação multifato do Azure (MFA), ele não poderá ser excluído.</span><span class="sxs-lookup"><span data-stu-id="43a2a-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="43a2a-110">Fazer com que o usuário altere seu método de autenticação padrão e exclua o número.</span><span class="sxs-lookup"><span data-stu-id="43a2a-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="43a2a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="43a2a-111">Permissions</span></span>

<span data-ttu-id="43a2a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43a2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="43a2a-114">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="43a2a-114">Permissions acting on self</span></span>

|<span data-ttu-id="43a2a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43a2a-115">Permission type</span></span>      | <span data-ttu-id="43a2a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43a2a-116">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="43a2a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43a2a-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="43a2a-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a2a-118">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="43a2a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43a2a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43a2a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43a2a-120">Not supported.</span></span> |
| <span data-ttu-id="43a2a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43a2a-121">Application</span></span>                            | <span data-ttu-id="43a2a-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43a2a-122">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="43a2a-123">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="43a2a-123">Permissions acting on other users</span></span>

|<span data-ttu-id="43a2a-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43a2a-124">Permission type</span></span>      | <span data-ttu-id="43a2a-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43a2a-125">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="43a2a-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43a2a-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="43a2a-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a2a-127">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="43a2a-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43a2a-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43a2a-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43a2a-129">Not supported.</span></span> |
| <span data-ttu-id="43a2a-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43a2a-130">Application</span></span>                            | <span data-ttu-id="43a2a-131">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a2a-131">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="43a2a-132">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="43a2a-132">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="43a2a-133">Administrador global</span><span class="sxs-lookup"><span data-stu-id="43a2a-133">Global admin</span></span>
* <span data-ttu-id="43a2a-134">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="43a2a-134">Privileged authentication admin</span></span>
* <span data-ttu-id="43a2a-135">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="43a2a-135">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="43a2a-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43a2a-136">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="43a2a-137">O valor correspondente ao phoneType a ser `id` excluído é um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="43a2a-137">The value of `id` corresponding to the phoneType to delete is one of the following:</span></span>
+ <span data-ttu-id="43a2a-138">`b6332ec1-7057-4abe-9331-3d72feddfe41` para excluir `alternateMobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="43a2a-138">`b6332ec1-7057-4abe-9331-3d72feddfe41` to delete the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="43a2a-139">`e37fc753-ff3b-4958-9484-eaa9425c82bc` para excluir `office` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="43a2a-139">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to delete the `office` **phoneType**.</span></span>
+ <span data-ttu-id="43a2a-140">`3179e48a-750b-4051-897c-87b9720928f7` para excluir `mobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="43a2a-140">`3179e48a-750b-4051-897c-87b9720928f7` to delete the `mobile` **phoneType**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43a2a-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43a2a-141">Request headers</span></span>

| <span data-ttu-id="43a2a-142">Nome</span><span class="sxs-lookup"><span data-stu-id="43a2a-142">Name</span></span>          | <span data-ttu-id="43a2a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="43a2a-143">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="43a2a-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="43a2a-144">Authorization</span></span> | <span data-ttu-id="43a2a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43a2a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43a2a-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43a2a-147">Request body</span></span>

<span data-ttu-id="43a2a-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43a2a-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43a2a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="43a2a-149">Response</span></span>

<span data-ttu-id="43a2a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43a2a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43a2a-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43a2a-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43a2a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43a2a-153">Request</span></span>

<span data-ttu-id="43a2a-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43a2a-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43a2a-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="43a2a-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="43a2a-156">C#</span><span class="sxs-lookup"><span data-stu-id="43a2a-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43a2a-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43a2a-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43a2a-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43a2a-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43a2a-159">Java</span><span class="sxs-lookup"><span data-stu-id="43a2a-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43a2a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="43a2a-160">Response</span></span>

<span data-ttu-id="43a2a-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43a2a-161">The following is an example of the response.</span></span>

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
