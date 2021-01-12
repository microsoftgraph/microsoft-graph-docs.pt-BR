---
title: Listar microsoftAuthenticatorAuthenticationMethods
description: Obter uma lista dos objetos microsoftAuthenticatorAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a880cb5ac1b0594b46f4de3649fc5a07060eb8be
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796720"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="a90ae-103">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="a90ae-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="a90ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a90ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a90ae-105">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a90ae-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a90ae-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a90ae-106">Permissions</span></span>

<span data-ttu-id="a90ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a90ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="a90ae-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="a90ae-109">Permissions acting on self</span></span>

|<span data-ttu-id="a90ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a90ae-110">Permission type</span></span>      | <span data-ttu-id="a90ae-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a90ae-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a90ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a90ae-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a90ae-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a90ae-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="a90ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a90ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a90ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a90ae-115">Not supported.</span></span> |
| <span data-ttu-id="a90ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a90ae-116">Application</span></span>                            | <span data-ttu-id="a90ae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a90ae-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="a90ae-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="a90ae-118">Permissions acting on other users</span></span>

|<span data-ttu-id="a90ae-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a90ae-119">Permission type</span></span>      | <span data-ttu-id="a90ae-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a90ae-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a90ae-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a90ae-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="a90ae-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a90ae-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a90ae-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a90ae-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a90ae-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a90ae-124">Not supported.</span></span> |
| <span data-ttu-id="a90ae-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a90ae-125">Application</span></span>                            | <span data-ttu-id="a90ae-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a90ae-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a90ae-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a90ae-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a90ae-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="a90ae-128">Global admin</span></span>
* <span data-ttu-id="a90ae-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="a90ae-129">Global reader</span></span>
* <span data-ttu-id="a90ae-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="a90ae-130">Privileged authentication admin</span></span>
* <span data-ttu-id="a90ae-131">Administrador de autenticação (vê apenas números de telefone com máscara)</span><span class="sxs-lookup"><span data-stu-id="a90ae-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="a90ae-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a90ae-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /user/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a90ae-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a90ae-133">Optional query parameters</span></span>

<span data-ttu-id="a90ae-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a90ae-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a90ae-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a90ae-135">Request headers</span></span>

|<span data-ttu-id="a90ae-136">Nome</span><span class="sxs-lookup"><span data-stu-id="a90ae-136">Name</span></span>|<span data-ttu-id="a90ae-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a90ae-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a90ae-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="a90ae-138">Authorization</span></span>|<span data-ttu-id="a90ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a90ae-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a90ae-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a90ae-141">Request body</span></span>

<span data-ttu-id="a90ae-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a90ae-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a90ae-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a90ae-143">Response</span></span>

<span data-ttu-id="a90ae-144">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a90ae-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a90ae-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a90ae-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a90ae-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a90ae-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/anirban@contoso.com/authentication/microsoftAuthenticatorMethods
```


### <a name="response"></a><span data-ttu-id="a90ae-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a90ae-147">Response</span></span>
<span data-ttu-id="a90ae-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a90ae-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.microsoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
      "id": "6803c096-c096-6803-96c0-036896c00368",
      "displayName": "Sandeep's iPhone",
      "deviceTag": "",
      "phoneAppVersion": "6.5.4",
      "createdDateTime": "2020-12-03T23:16:12Z"
    }
  ]
}
```

