---
title: Excluir windowsHelloForBusinessAuthenticationMethod
description: Exclui um objeto windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d0412cc7bdc1ed20ddba80d70b992d3859ca507c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873315"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="90473-103">Excluir windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="90473-103">Delete windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="90473-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90473-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90473-105">Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="90473-105">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90473-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90473-106">Permissions</span></span>

<span data-ttu-id="90473-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90473-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="90473-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="90473-109">Permissions acting on self</span></span>

|<span data-ttu-id="90473-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90473-110">Permission type</span></span>      | <span data-ttu-id="90473-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90473-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="90473-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90473-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="90473-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90473-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="90473-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90473-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90473-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90473-115">Not supported.</span></span> |
| <span data-ttu-id="90473-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90473-116">Application</span></span>                            | <span data-ttu-id="90473-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90473-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="90473-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="90473-118">Permissions acting on other users</span></span>

|<span data-ttu-id="90473-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90473-119">Permission type</span></span>      | <span data-ttu-id="90473-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90473-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="90473-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90473-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="90473-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90473-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="90473-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90473-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90473-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90473-124">Not supported.</span></span> |
| <span data-ttu-id="90473-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90473-125">Application</span></span>                            | <span data-ttu-id="90473-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90473-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="90473-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="90473-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="90473-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="90473-128">Global admin</span></span>
* <span data-ttu-id="90473-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="90473-129">Privileged authentication admin</span></span>
* <span data-ttu-id="90473-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="90473-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="90473-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90473-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="90473-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90473-132">Request headers</span></span>
|<span data-ttu-id="90473-133">Nome</span><span class="sxs-lookup"><span data-stu-id="90473-133">Name</span></span>|<span data-ttu-id="90473-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="90473-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="90473-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="90473-135">Authorization</span></span>|<span data-ttu-id="90473-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90473-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90473-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90473-138">Request body</span></span>
<span data-ttu-id="90473-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90473-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90473-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="90473-140">Response</span></span>

<span data-ttu-id="90473-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90473-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="90473-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90473-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90473-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90473-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="90473-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="90473-144">Response</span></span>
<span data-ttu-id="90473-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="90473-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

