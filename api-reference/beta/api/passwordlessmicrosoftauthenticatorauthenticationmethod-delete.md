---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Exclui um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e7931c0524662397e25f97a0c53426b243226be
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457517"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="be6bb-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="be6bb-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="be6bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be6bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be6bb-105">Exclui o objeto de [método de entrada de telefone sem senha do autenticador da Microsoft](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="be6bb-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="be6bb-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="be6bb-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="be6bb-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="be6bb-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="permissions"></a><span data-ttu-id="be6bb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="be6bb-108">Permissions</span></span>
<span data-ttu-id="be6bb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be6bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be6bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be6bb-111">Permission type</span></span>|<span data-ttu-id="be6bb-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="be6bb-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="be6bb-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be6bb-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="be6bb-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be6bb-114">Delegated (work or school account)</span></span>|<span data-ttu-id="be6bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6bb-115">Not supported.</span></span>|<span data-ttu-id="be6bb-116">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="be6bb-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="be6bb-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be6bb-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be6bb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6bb-118">Not supported.</span></span>|<span data-ttu-id="be6bb-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6bb-119">Not supported.</span></span>
|<span data-ttu-id="be6bb-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be6bb-120">Application</span></span>|<span data-ttu-id="be6bb-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6bb-121">Not supported.</span></span>|<span data-ttu-id="be6bb-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6bb-122">Not supported.</span></span>

<span data-ttu-id="be6bb-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="be6bb-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="be6bb-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="be6bb-124">Global admin</span></span>
* <span data-ttu-id="be6bb-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="be6bb-125">Global reader</span></span>
* <span data-ttu-id="be6bb-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="be6bb-126">Privileged authentication admin</span></span>
* <span data-ttu-id="be6bb-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="be6bb-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="be6bb-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be6bb-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="be6bb-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be6bb-129">Request headers</span></span>
|<span data-ttu-id="be6bb-130">Nome</span><span class="sxs-lookup"><span data-stu-id="be6bb-130">Name</span></span>|<span data-ttu-id="be6bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be6bb-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="be6bb-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="be6bb-132">Authorization</span></span>|<span data-ttu-id="be6bb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be6bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be6bb-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be6bb-135">Request body</span></span>
<span data-ttu-id="be6bb-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be6bb-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be6bb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="be6bb-137">Response</span></span>

<span data-ttu-id="be6bb-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be6bb-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be6bb-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be6bb-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be6bb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be6bb-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="be6bb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="be6bb-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="be6bb-143">C#</span><span class="sxs-lookup"><span data-stu-id="be6bb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be6bb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be6bb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be6bb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be6bb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="be6bb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="be6bb-146">Response</span></span>
<span data-ttu-id="be6bb-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be6bb-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

