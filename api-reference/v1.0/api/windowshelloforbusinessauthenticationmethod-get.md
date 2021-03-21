---
title: Obter windowsHelloForBusinessAuthenticationMethod
description: Leia as propriedades e as relações de um objeto windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 892c94dc8d5704e78910f323d6940e23e9b8471d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964578"
---
# <a name="get-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="c323a-103">Obter windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c323a-103">Get windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="c323a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c323a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c323a-105">Leia as propriedades e as relações de um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c323a-105">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c323a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c323a-106">Permissions</span></span>

<span data-ttu-id="c323a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c323a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="c323a-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="c323a-109">Permissions acting on self</span></span>

|<span data-ttu-id="c323a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c323a-110">Permission type</span></span>      | <span data-ttu-id="c323a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c323a-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="c323a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c323a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c323a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c323a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="c323a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c323a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c323a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c323a-115">Not supported.</span></span> |
| <span data-ttu-id="c323a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c323a-116">Application</span></span>                            | <span data-ttu-id="c323a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c323a-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="c323a-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="c323a-118">Permissions acting on other users</span></span>

|<span data-ttu-id="c323a-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c323a-119">Permission type</span></span>      | <span data-ttu-id="c323a-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c323a-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="c323a-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c323a-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="c323a-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c323a-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c323a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c323a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c323a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c323a-124">Not supported.</span></span> |
| <span data-ttu-id="c323a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c323a-125">Application</span></span>                            | <span data-ttu-id="c323a-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c323a-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="c323a-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="c323a-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="c323a-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c323a-128">Global admin</span></span>
* <span data-ttu-id="c323a-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="c323a-129">Global reader</span></span>
* <span data-ttu-id="c323a-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c323a-130">Privileged authentication admin</span></span>
* <span data-ttu-id="c323a-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="c323a-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="c323a-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c323a-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c323a-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c323a-133">Optional query parameters</span></span>

<span data-ttu-id="c323a-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c323a-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c323a-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c323a-135">Request headers</span></span>
|<span data-ttu-id="c323a-136">Nome</span><span class="sxs-lookup"><span data-stu-id="c323a-136">Name</span></span>|<span data-ttu-id="c323a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c323a-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c323a-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="c323a-138">Authorization</span></span>|<span data-ttu-id="c323a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c323a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c323a-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c323a-141">Request body</span></span>
<span data-ttu-id="c323a-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c323a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c323a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c323a-143">Response</span></span>

<span data-ttu-id="c323a-144">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c323a-144">If successful, this method returns a `200 OK` response code and a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c323a-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c323a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c323a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c323a-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="c323a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c323a-147">Response</span></span>
<span data-ttu-id="c323a-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c323a-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
  }
}
```

