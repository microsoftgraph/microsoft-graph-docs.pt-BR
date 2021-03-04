---
title: Listar fido2AuthenticationMethod
description: Recupere uma lista dos objetos fido2AuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 57e63c083e75a84eff13ffc5094041224bdd43d7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436054"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="c4095-103">Listar fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c4095-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="c4095-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4095-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4095-105">Recupere uma lista dos objetos [fido2 security key authentication method](../resources/fido2authenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c4095-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4095-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4095-106">Permissions</span></span>
<span data-ttu-id="c4095-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4095-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4095-109">Permission type</span></span>|<span data-ttu-id="c4095-110">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="c4095-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="c4095-111">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="c4095-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="c4095-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4095-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4095-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4095-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="c4095-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4095-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c4095-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4095-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4095-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4095-116">Not supported.</span></span> | <span data-ttu-id="c4095-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4095-117">Not supported.</span></span> |
| <span data-ttu-id="c4095-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4095-118">Application</span></span>                            | <span data-ttu-id="c4095-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c4095-119">Not applicable.</span></span> | <span data-ttu-id="c4095-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4095-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="c4095-121">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="c4095-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c4095-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c4095-122">Global admin</span></span>
* <span data-ttu-id="c4095-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="c4095-123">Global reader</span></span>
* <span data-ttu-id="c4095-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c4095-124">Privileged authentication admin</span></span>
* <span data-ttu-id="c4095-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="c4095-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c4095-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4095-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4095-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4095-127">Optional query parameters</span></span>
<span data-ttu-id="c4095-128">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4095-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4095-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4095-129">Request headers</span></span>
|<span data-ttu-id="c4095-130">Nome</span><span class="sxs-lookup"><span data-stu-id="c4095-130">Name</span></span>|<span data-ttu-id="c4095-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4095-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4095-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4095-132">Authorization</span></span>|<span data-ttu-id="c4095-133">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c4095-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4095-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4095-134">Request body</span></span>
<span data-ttu-id="c4095-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4095-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4095-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4095-136">Response</span></span>

<span data-ttu-id="c4095-137">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4095-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4095-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4095-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4095-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4095-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4095-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4095-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```
# <a name="c"></a>[<span data-ttu-id="c4095-141">C#</span><span class="sxs-lookup"><span data-stu-id="c4095-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4095-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4095-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4095-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4095-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4095-144">Java</span><span class="sxs-lookup"><span data-stu-id="c4095-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4095-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4095-145">Response</span></span>
<span data-ttu-id="c4095-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4095-146">The following is an example of the response.</span></span>

<span data-ttu-id="c4095-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4095-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

