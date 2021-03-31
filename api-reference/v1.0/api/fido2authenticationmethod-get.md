---
title: Obter fido2AuthenticationMethod
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b641e1c2afdbf01a3999c50f76497ac7a1417382
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467957"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="129b4-103">Obter fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="129b4-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="129b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="129b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="129b4-105">Recupere o único objeto do método de autenticação de chave de segurança [FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="129b4-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="129b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="129b4-106">Permissions</span></span>

<span data-ttu-id="129b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="129b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="129b4-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="129b4-109">Permissions acting on self</span></span>

|<span data-ttu-id="129b4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="129b4-110">Permission type</span></span>      | <span data-ttu-id="129b4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="129b4-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="129b4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="129b4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="129b4-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="129b4-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="129b4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="129b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="129b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="129b4-115">Not supported.</span></span> |
| <span data-ttu-id="129b4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="129b4-116">Application</span></span>                            | <span data-ttu-id="129b4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="129b4-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="129b4-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="129b4-118">Permissions acting on other users</span></span>

|<span data-ttu-id="129b4-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="129b4-119">Permission type</span></span>      | <span data-ttu-id="129b4-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="129b4-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="129b4-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="129b4-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="129b4-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="129b4-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="129b4-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="129b4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="129b4-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="129b4-124">Not supported.</span></span> |
| <span data-ttu-id="129b4-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="129b4-125">Application</span></span>                            | <span data-ttu-id="129b4-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="129b4-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="129b4-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="129b4-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="129b4-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="129b4-128">Global admin</span></span>
* <span data-ttu-id="129b4-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="129b4-129">Global reader</span></span>
* <span data-ttu-id="129b4-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="129b4-130">Privileged authentication admin</span></span>
* <span data-ttu-id="129b4-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="129b4-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="129b4-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="129b4-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="129b4-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="129b4-133">Request headers</span></span>
|<span data-ttu-id="129b4-134">Nome</span><span class="sxs-lookup"><span data-stu-id="129b4-134">Name</span></span>|<span data-ttu-id="129b4-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="129b4-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="129b4-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="129b4-136">Authorization</span></span>|<span data-ttu-id="129b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="129b4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="129b4-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="129b4-139">Request body</span></span>
<span data-ttu-id="129b4-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="129b4-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="129b4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="129b4-141">Response</span></span>

<span data-ttu-id="129b4-142">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="129b4-142">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="129b4-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="129b4-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="129b4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="129b4-144">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```

### <a name="response"></a><span data-ttu-id="129b4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="129b4-145">Response</span></span>
<span data-ttu-id="129b4-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="129b4-146">The following is an example of the response.</span></span>

<span data-ttu-id="129b4-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="129b4-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

