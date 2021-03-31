---
title: Listar fido2AuthenticationMethod
description: Recupere uma lista dos objetos fido2AuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 166ac533d85e43fdc413f614ce848cdbdb5c56e7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469266"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="dc588-103">Listar fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dc588-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="dc588-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc588-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc588-105">Recupere uma lista dos objetos [fido2 security key authentication method](../resources/fido2authenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="dc588-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc588-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc588-106">Permissions</span></span>

<span data-ttu-id="dc588-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="dc588-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="dc588-109">Permissions acting on self</span></span>

|<span data-ttu-id="dc588-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc588-110">Permission type</span></span>      | <span data-ttu-id="dc588-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc588-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="dc588-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc588-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc588-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc588-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="dc588-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc588-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc588-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc588-115">Not supported.</span></span> |
| <span data-ttu-id="dc588-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc588-116">Application</span></span>                            | <span data-ttu-id="dc588-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc588-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="dc588-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="dc588-118">Permissions acting on other users</span></span>

|<span data-ttu-id="dc588-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc588-119">Permission type</span></span>      | <span data-ttu-id="dc588-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc588-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="dc588-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc588-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc588-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc588-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="dc588-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc588-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc588-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc588-124">Not supported.</span></span> |
| <span data-ttu-id="dc588-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc588-125">Application</span></span>                            | <span data-ttu-id="dc588-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc588-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="dc588-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="dc588-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="dc588-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="dc588-128">Global admin</span></span>
* <span data-ttu-id="dc588-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="dc588-129">Global reader</span></span>
* <span data-ttu-id="dc588-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="dc588-130">Privileged authentication admin</span></span>
* <span data-ttu-id="dc588-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="dc588-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="dc588-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc588-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc588-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc588-133">Optional query parameters</span></span>
<span data-ttu-id="dc588-134">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc588-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc588-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc588-135">Request headers</span></span>
|<span data-ttu-id="dc588-136">Nome</span><span class="sxs-lookup"><span data-stu-id="dc588-136">Name</span></span>|<span data-ttu-id="dc588-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc588-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc588-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc588-138">Authorization</span></span>|<span data-ttu-id="dc588-139">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="dc588-139">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc588-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc588-140">Request body</span></span>
<span data-ttu-id="dc588-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc588-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc588-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc588-142">Response</span></span>

<span data-ttu-id="dc588-143">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc588-143">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc588-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc588-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc588-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc588-145">Request</span></span>


``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2Methods
```

### <a name="response"></a><span data-ttu-id="dc588-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc588-146">Response</span></span>
<span data-ttu-id="dc588-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc588-147">The following is an example of the response.</span></span>

<span data-ttu-id="dc588-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc588-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.fido2AuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
      "id": "_jpuR-TGZgk6aQCLF3BQjA2",
      "displayName": "Blue key",
      "creationDateTime": "2020-08-10T06:25:38Z",
      "aaGuid": "c5ef55ff-ad9a-4b9f-b580-ababafe026d0",
      "model": "USB key",
      "attestationCertificates": [
          "b479e7652167f574296e76bfa76731b8ccd22ed7"
      ],
      "attestationLevel": "attested"
    }
  ]
}
```

