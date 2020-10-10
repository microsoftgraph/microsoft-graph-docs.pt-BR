---
title: Excluir phoneAuthenticationMethod
description: Exclua o método de autenticação de telefone de um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 83d83f0e1c298484a69a72eebc57d02feeb9738d
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417839"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="1137d-103">Excluir phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1137d-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="1137d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1137d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1137d-105">Exclua o [método de autenticação de telefone](../resources/phoneauthenticationmethod.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1137d-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="1137d-106">**Observação:** Isso removerá o número de telefone do usuário e não poderá mais usar o número para autenticação, seja via SMS ou chamadas de voz.</span><span class="sxs-lookup"><span data-stu-id="1137d-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="1137d-107">Lembre-se de que um usuário não pode ter um `alternateMobile` número sem um `mobile` número.</span><span class="sxs-lookup"><span data-stu-id="1137d-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="1137d-108">Se você deseja remover um `mobile` número de um usuário que também tem um `alternateMobile` número, primeiro [atualize](phoneauthenticationmethod-update.md) o `mobile` número para o novo número e, em seguida, exclua o `alternateMobile` número.</span><span class="sxs-lookup"><span data-stu-id="1137d-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="1137d-109">Se o número de telefone é o método de autenticação de autenticação multifator do Azure (MFA) padrão do usuário, ele não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="1137d-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="1137d-110">Peça para o usuário alterar o método de autenticação padrão e, em seguida, exclua o número.</span><span class="sxs-lookup"><span data-stu-id="1137d-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="1137d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1137d-111">Permissions</span></span>

<span data-ttu-id="1137d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1137d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1137d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1137d-114">Permission type</span></span>                        | <span data-ttu-id="1137d-115">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1137d-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="1137d-116">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1137d-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="1137d-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1137d-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1137d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1137d-118">Not supported.</span></span> | <span data-ttu-id="1137d-119">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1137d-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1137d-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1137d-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1137d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1137d-121">Not supported.</span></span> | <span data-ttu-id="1137d-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1137d-122">Not supported.</span></span> |
| <span data-ttu-id="1137d-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1137d-123">Application</span></span>                            | <span data-ttu-id="1137d-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1137d-124">Not supported.</span></span> | <span data-ttu-id="1137d-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1137d-125">Not supported.</span></span> |

<span data-ttu-id="1137d-126">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="1137d-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1137d-127">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1137d-127">Global admin</span></span>
* <span data-ttu-id="1137d-128">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="1137d-128">Privileged authentication admin</span></span>
* <span data-ttu-id="1137d-129">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="1137d-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1137d-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1137d-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1137d-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1137d-131">Request headers</span></span>

| <span data-ttu-id="1137d-132">Nome</span><span class="sxs-lookup"><span data-stu-id="1137d-132">Name</span></span>          | <span data-ttu-id="1137d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1137d-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1137d-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="1137d-134">Authorization</span></span> | <span data-ttu-id="1137d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1137d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1137d-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1137d-137">Request body</span></span>

<span data-ttu-id="1137d-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1137d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1137d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1137d-139">Response</span></span>

<span data-ttu-id="1137d-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1137d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1137d-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1137d-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1137d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1137d-143">Request</span></span>

<span data-ttu-id="1137d-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1137d-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1137d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1137d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="1137d-146">C#</span><span class="sxs-lookup"><span data-stu-id="1137d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1137d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1137d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1137d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1137d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1137d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1137d-149">Response</span></span>

<span data-ttu-id="1137d-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1137d-150">The following is an example of the response.</span></span>

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