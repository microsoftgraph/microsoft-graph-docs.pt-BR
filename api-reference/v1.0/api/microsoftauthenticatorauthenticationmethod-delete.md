---
title: Excluir microsoftAuthenticatorAuthenticationMethod
description: Exclui um objeto microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 848aa51dfa82d192b48c768a659f2da17fa71e94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948964"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="2eae1-103">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2eae1-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="2eae1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2eae1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2eae1-105">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="2eae1-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2eae1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2eae1-106">Permissions</span></span>

<span data-ttu-id="2eae1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eae1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="2eae1-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="2eae1-109">Permissions acting on self</span></span>

|<span data-ttu-id="2eae1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eae1-110">Permission type</span></span>      | <span data-ttu-id="2eae1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2eae1-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="2eae1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eae1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2eae1-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2eae1-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="2eae1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eae1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eae1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eae1-115">Not supported.</span></span> |
| <span data-ttu-id="2eae1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eae1-116">Application</span></span>                            | <span data-ttu-id="2eae1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eae1-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="2eae1-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="2eae1-118">Permissions acting on other users</span></span>

|<span data-ttu-id="2eae1-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eae1-119">Permission type</span></span>      | <span data-ttu-id="2eae1-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2eae1-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="2eae1-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eae1-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="2eae1-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eae1-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2eae1-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eae1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eae1-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eae1-124">Not supported.</span></span> |
| <span data-ttu-id="2eae1-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eae1-125">Application</span></span>                            | <span data-ttu-id="2eae1-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eae1-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="2eae1-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="2eae1-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="2eae1-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2eae1-128">Global admin</span></span>
* <span data-ttu-id="2eae1-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="2eae1-129">Privileged authentication admin</span></span>
* <span data-ttu-id="2eae1-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="2eae1-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2eae1-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2eae1-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="2eae1-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2eae1-132">Request headers</span></span>
|<span data-ttu-id="2eae1-133">Nome</span><span class="sxs-lookup"><span data-stu-id="2eae1-133">Name</span></span>|<span data-ttu-id="2eae1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eae1-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2eae1-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="2eae1-135">Authorization</span></span>|<span data-ttu-id="2eae1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2eae1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eae1-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2eae1-138">Request body</span></span>
<span data-ttu-id="2eae1-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2eae1-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2eae1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eae1-140">Response</span></span>

<span data-ttu-id="2eae1-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2eae1-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2eae1-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2eae1-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2eae1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2eae1-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="2eae1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eae1-144">Response</span></span>
<span data-ttu-id="2eae1-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2eae1-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

