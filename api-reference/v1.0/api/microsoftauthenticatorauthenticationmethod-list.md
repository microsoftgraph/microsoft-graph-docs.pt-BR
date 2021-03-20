---
title: Listar microsoftAuthenticatorAuthenticationMethods
description: Obter uma lista dos objetos microsoftAuthenticatorAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 66fca8025edf86fb9b84632eed0ab3ff67d5ddf9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948962"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="9126a-103">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="9126a-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="9126a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9126a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9126a-105">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9126a-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="9126a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9126a-106">Permissions</span></span>

<span data-ttu-id="9126a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9126a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9126a-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="9126a-109">Permissions acting on self</span></span>

|<span data-ttu-id="9126a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9126a-110">Permission type</span></span>      | <span data-ttu-id="9126a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9126a-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9126a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9126a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9126a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9126a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9126a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9126a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9126a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9126a-115">Not supported.</span></span> |
| <span data-ttu-id="9126a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9126a-116">Application</span></span>                            | <span data-ttu-id="9126a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9126a-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9126a-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="9126a-118">Permissions acting on other users</span></span>

|<span data-ttu-id="9126a-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9126a-119">Permission type</span></span>      | <span data-ttu-id="9126a-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9126a-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="9126a-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9126a-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9126a-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9126a-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9126a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9126a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9126a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9126a-124">Not supported.</span></span> |
| <span data-ttu-id="9126a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9126a-125">Application</span></span>                            | <span data-ttu-id="9126a-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9126a-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9126a-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9126a-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9126a-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9126a-128">Global admin</span></span>
* <span data-ttu-id="9126a-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="9126a-129">Global reader</span></span>
* <span data-ttu-id="9126a-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="9126a-130">Privileged authentication admin</span></span>
* <span data-ttu-id="9126a-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="9126a-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="9126a-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9126a-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9126a-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9126a-133">Optional query parameters</span></span>

<span data-ttu-id="9126a-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9126a-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9126a-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9126a-135">Request headers</span></span>

|<span data-ttu-id="9126a-136">Nome</span><span class="sxs-lookup"><span data-stu-id="9126a-136">Name</span></span>|<span data-ttu-id="9126a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9126a-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9126a-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="9126a-138">Authorization</span></span>|<span data-ttu-id="9126a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9126a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9126a-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9126a-141">Request body</span></span>

<span data-ttu-id="9126a-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9126a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9126a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9126a-143">Response</span></span>

<span data-ttu-id="9126a-144">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9126a-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9126a-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9126a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9126a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9126a-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/sandeep@contoso.com/authentication/microsoftAuthenticatorMethods
```


### <a name="response"></a><span data-ttu-id="9126a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9126a-147">Response</span></span>
<span data-ttu-id="9126a-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9126a-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

