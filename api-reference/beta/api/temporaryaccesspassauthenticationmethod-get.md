---
title: Obter temporaryAccessPassAuthenticationMethod
description: Leia as propriedades e os relacionamentos de um objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 154afeae29769fb29122f6f35503b919bfad0e7e
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272591"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="a78ca-103">Obter temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a78ca-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="a78ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a78ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a78ca-105">Recupere o único objeto  [temporaryAccessPassAuthenticationMethod de um](../resources/temporaryaccesspassauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="a78ca-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a78ca-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a78ca-106">Permissions</span></span>
<span data-ttu-id="a78ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a78ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="a78ca-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="a78ca-109">Permissions acting on self</span></span>

|<span data-ttu-id="a78ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a78ca-110">Permission type</span></span>      | <span data-ttu-id="a78ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a78ca-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a78ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a78ca-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a78ca-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a78ca-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="a78ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a78ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a78ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a78ca-115">Not supported.</span></span> |
| <span data-ttu-id="a78ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a78ca-116">Application</span></span>                            | <span data-ttu-id="a78ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a78ca-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="a78ca-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="a78ca-118">Permissions acting on other users</span></span>

|<span data-ttu-id="a78ca-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a78ca-119">Permission type</span></span>      | <span data-ttu-id="a78ca-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a78ca-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a78ca-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a78ca-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="a78ca-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a78ca-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a78ca-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a78ca-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a78ca-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a78ca-124">Not supported.</span></span> |
| <span data-ttu-id="a78ca-125">Application</span><span class="sxs-lookup"><span data-stu-id="a78ca-125">Application</span></span>                            | <span data-ttu-id="a78ca-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a78ca-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a78ca-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a78ca-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a78ca-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a78ca-128">Global admin</span></span>
* <span data-ttu-id="a78ca-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="a78ca-129">Global reader</span></span>
* <span data-ttu-id="a78ca-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="a78ca-130">Privileged authentication admin</span></span>
* <span data-ttu-id="a78ca-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="a78ca-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="a78ca-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a78ca-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="a78ca-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a78ca-133">Request headers</span></span>
|<span data-ttu-id="a78ca-134">Nome</span><span class="sxs-lookup"><span data-stu-id="a78ca-134">Name</span></span>|<span data-ttu-id="a78ca-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a78ca-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a78ca-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="a78ca-136">Authorization</span></span>|<span data-ttu-id="a78ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a78ca-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="a78ca-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a78ca-139">Request body</span></span>
<span data-ttu-id="a78ca-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a78ca-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a78ca-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a78ca-141">Response</span></span>

<span data-ttu-id="a78ca-142">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a78ca-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a78ca-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a78ca-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a78ca-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a78ca-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```


### <a name="response"></a><span data-ttu-id="a78ca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a78ca-145">Response</span></span>
<span data-ttu-id="a78ca-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a78ca-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
    "temporaryAccessPass": null,
    "createdDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "lifetimeInMinutes": "Integer",
    "isUsableOnce": "Boolean",
    "isUsable": "Boolean",
    "methodUsabilityReason": "String"
  }
}
```
