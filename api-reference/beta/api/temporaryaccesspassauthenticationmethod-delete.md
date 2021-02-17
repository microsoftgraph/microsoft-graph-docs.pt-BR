---
title: Excluir temporaryAccessPassAuthenticationMethod
description: Exclui um objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0aefe7a59e9fa0a13420182995bb60b0b7fe4121
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272592"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="80b56-103">Excluir temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="80b56-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="80b56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80b56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80b56-105">[Exclua um objeto temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="80b56-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="80b56-106">Embora a passagem de acesso temporário atual do usuário seja válida, ela precisa ser excluída antes que um novo Acesso Temporário possa ser criado no usuário.</span><span class="sxs-lookup"><span data-stu-id="80b56-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="80b56-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="80b56-107">Permissions</span></span>
<span data-ttu-id="80b56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="80b56-110">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="80b56-110">Permissions acting on self</span></span>

|<span data-ttu-id="80b56-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80b56-111">Permission type</span></span>      | <span data-ttu-id="80b56-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80b56-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="80b56-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80b56-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="80b56-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80b56-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="80b56-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80b56-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80b56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80b56-116">Not supported.</span></span> |
| <span data-ttu-id="80b56-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80b56-117">Application</span></span>                            | <span data-ttu-id="80b56-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80b56-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="80b56-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="80b56-119">Permissions acting on other users</span></span>

|<span data-ttu-id="80b56-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80b56-120">Permission type</span></span>      | <span data-ttu-id="80b56-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80b56-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="80b56-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80b56-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="80b56-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80b56-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="80b56-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80b56-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80b56-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80b56-125">Not supported.</span></span> |
| <span data-ttu-id="80b56-126">Application</span><span class="sxs-lookup"><span data-stu-id="80b56-126">Application</span></span>                            | <span data-ttu-id="80b56-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80b56-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="80b56-128">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="80b56-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="80b56-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="80b56-129">Global admin</span></span>
* <span data-ttu-id="80b56-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="80b56-130">Privileged authentication admin</span></span>
* <span data-ttu-id="80b56-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="80b56-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="80b56-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80b56-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80b56-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80b56-133">Request headers</span></span>
|<span data-ttu-id="80b56-134">Nome</span><span class="sxs-lookup"><span data-stu-id="80b56-134">Name</span></span>|<span data-ttu-id="80b56-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="80b56-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="80b56-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="80b56-136">Authorization</span></span>|<span data-ttu-id="80b56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80b56-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80b56-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80b56-139">Request body</span></span>
<span data-ttu-id="80b56-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80b56-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80b56-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="80b56-141">Response</span></span>

<span data-ttu-id="80b56-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80b56-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80b56-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="80b56-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80b56-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80b56-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```


### <a name="response"></a><span data-ttu-id="80b56-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="80b56-146">Response</span></span>
<span data-ttu-id="80b56-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="80b56-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```