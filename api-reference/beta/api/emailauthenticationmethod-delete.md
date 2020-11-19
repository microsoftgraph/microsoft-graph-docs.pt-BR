---
title: Excluir emailAuthenticationMethod
description: Exclui um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0602bdc0e619e87bc2d4f70d5ab668bc31066163
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352163"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="6d0df-103">Excluir emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6d0df-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="6d0df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d0df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d0df-105">Exclui o objeto de [método de autenticação de email](../resources/emailauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6d0df-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d0df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d0df-106">Permissions</span></span>
<span data-ttu-id="6d0df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d0df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d0df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d0df-109">Permission type</span></span>|<span data-ttu-id="6d0df-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d0df-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="6d0df-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d0df-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="6d0df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d0df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d0df-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d0df-113">Not supported.</span></span>|<span data-ttu-id="6d0df-114">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d0df-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="6d0df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d0df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d0df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d0df-116">Not supported.</span></span>|<span data-ttu-id="6d0df-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d0df-117">Not supported.</span></span>
|<span data-ttu-id="6d0df-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d0df-118">Application</span></span>|<span data-ttu-id="6d0df-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d0df-119">Not supported.</span></span>|<span data-ttu-id="6d0df-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d0df-120">Not supported.</span></span>

<span data-ttu-id="6d0df-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="6d0df-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="6d0df-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6d0df-122">Global admin</span></span>
* <span data-ttu-id="6d0df-123">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="6d0df-123">Privileged authentication admin</span></span>
* <span data-ttu-id="6d0df-124">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="6d0df-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6d0df-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d0df-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d0df-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d0df-126">Request headers</span></span>
|<span data-ttu-id="6d0df-127">Nome</span><span class="sxs-lookup"><span data-stu-id="6d0df-127">Name</span></span>|<span data-ttu-id="6d0df-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d0df-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6d0df-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d0df-129">Authorization</span></span>|<span data-ttu-id="6d0df-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d0df-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d0df-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d0df-132">Request body</span></span>
<span data-ttu-id="6d0df-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d0df-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d0df-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d0df-134">Response</span></span>

<span data-ttu-id="6d0df-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d0df-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d0df-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6d0df-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d0df-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d0df-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6d0df-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d0df-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="6d0df-140">C#</span><span class="sxs-lookup"><span data-stu-id="6d0df-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d0df-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d0df-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d0df-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d0df-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d0df-143">Java</span><span class="sxs-lookup"><span data-stu-id="6d0df-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6d0df-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d0df-144">Response</span></span>
<span data-ttu-id="6d0df-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d0df-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

