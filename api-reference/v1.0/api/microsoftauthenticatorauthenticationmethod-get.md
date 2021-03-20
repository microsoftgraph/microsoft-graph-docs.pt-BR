---
title: Obter microsoftAuthenticatorAuthenticationMethod
description: Leia as propriedades e as relações de um objeto microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59a4fadb4658ee21f094bdc38e3b1eff6bd5cb7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948963"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="20909-103">Obter microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="20909-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="20909-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20909-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20909-105">Leia as propriedades e as relações de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="20909-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20909-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20909-106">Permissions</span></span>

<span data-ttu-id="20909-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="20909-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="20909-109">Permissions acting on self</span></span>

|<span data-ttu-id="20909-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20909-110">Permission type</span></span>      | <span data-ttu-id="20909-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20909-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="20909-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20909-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="20909-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20909-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="20909-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20909-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20909-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20909-115">Not supported.</span></span> |
| <span data-ttu-id="20909-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20909-116">Application</span></span>                            | <span data-ttu-id="20909-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20909-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="20909-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="20909-118">Permissions acting on other users</span></span>

|<span data-ttu-id="20909-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20909-119">Permission type</span></span>      | <span data-ttu-id="20909-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20909-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="20909-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20909-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="20909-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20909-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="20909-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20909-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20909-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20909-124">Not supported.</span></span> |
| <span data-ttu-id="20909-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20909-125">Application</span></span>                            | <span data-ttu-id="20909-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20909-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="20909-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="20909-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="20909-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="20909-128">Global admin</span></span>
* <span data-ttu-id="20909-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="20909-129">Global reader</span></span>
* <span data-ttu-id="20909-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="20909-130">Privileged authentication admin</span></span>
* <span data-ttu-id="20909-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="20909-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="20909-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20909-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20909-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20909-133">Optional query parameters</span></span>
<span data-ttu-id="20909-134">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20909-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="20909-135">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="20909-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20909-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20909-136">Request headers</span></span>
|<span data-ttu-id="20909-137">Nome</span><span class="sxs-lookup"><span data-stu-id="20909-137">Name</span></span>|<span data-ttu-id="20909-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="20909-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20909-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="20909-139">Authorization</span></span>|<span data-ttu-id="20909-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20909-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20909-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20909-142">Request body</span></span>
<span data-ttu-id="20909-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20909-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20909-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20909-144">Response</span></span>

<span data-ttu-id="20909-145">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20909-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20909-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20909-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20909-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20909-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="20909-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="20909-148">Response</span></span>
<span data-ttu-id="20909-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="20909-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
    "id": "6803c096-c096-6803-96c0-036896c00368",
    "displayName": "Sandeep's iPhone",
    "deviceTag": "",
    "phoneAppVersion": "6.5.4",
    "createdDateTime": "2020-12-03T23:16:12Z"
  }
}
```
