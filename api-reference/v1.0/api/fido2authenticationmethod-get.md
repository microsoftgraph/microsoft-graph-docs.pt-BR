---
title: Obter fido2AuthenticationMethod
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b13b9502c1587fcef5a20a07cc4b57d0300f91ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964590"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="b3742-103">Obter fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3742-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="b3742-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3742-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3742-105">Recupere o único objeto do método de autenticação de chave de segurança [FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="b3742-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3742-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3742-106">Permissions</span></span>

<span data-ttu-id="b3742-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b3742-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="b3742-109">Permissions acting on self</span></span>

|<span data-ttu-id="b3742-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3742-110">Permission type</span></span>      | <span data-ttu-id="b3742-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3742-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b3742-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3742-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3742-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3742-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b3742-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3742-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3742-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3742-115">Not supported.</span></span> |
| <span data-ttu-id="b3742-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3742-116">Application</span></span>                            | <span data-ttu-id="b3742-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3742-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b3742-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="b3742-118">Permissions acting on other users</span></span>

|<span data-ttu-id="b3742-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3742-119">Permission type</span></span>      | <span data-ttu-id="b3742-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3742-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b3742-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3742-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3742-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3742-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b3742-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3742-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3742-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3742-124">Not supported.</span></span> |
| <span data-ttu-id="b3742-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3742-125">Application</span></span>                            | <span data-ttu-id="b3742-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3742-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b3742-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b3742-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b3742-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b3742-128">Global admin</span></span>
* <span data-ttu-id="b3742-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="b3742-129">Global reader</span></span>
* <span data-ttu-id="b3742-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="b3742-130">Privileged authentication admin</span></span>
* <span data-ttu-id="b3742-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="b3742-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="b3742-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3742-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3742-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3742-133">Request headers</span></span>
|<span data-ttu-id="b3742-134">Nome</span><span class="sxs-lookup"><span data-stu-id="b3742-134">Name</span></span>|<span data-ttu-id="b3742-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3742-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3742-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3742-136">Authorization</span></span>|<span data-ttu-id="b3742-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3742-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3742-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3742-139">Request body</span></span>
<span data-ttu-id="b3742-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3742-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3742-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3742-141">Response</span></span>

<span data-ttu-id="b3742-142">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3742-142">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3742-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b3742-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3742-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3742-144">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```

### <a name="response"></a><span data-ttu-id="b3742-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3742-145">Response</span></span>
<span data-ttu-id="b3742-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3742-146">The following is an example of the response.</span></span>

<span data-ttu-id="b3742-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b3742-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
  }
}
```

