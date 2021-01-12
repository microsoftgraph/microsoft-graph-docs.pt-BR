---
title: Listar fido2AuthenticationMethod
description: Recupere uma lista dos objetos fido2AuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d7fe1e06dc9cd2e1c97354ae16b6d1582fbe4834
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796512"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="00317-103">Listar fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="00317-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="00317-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00317-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00317-105">Recupere uma lista de objetos do Método de Autenticação de Chave de Segurança [FIDO2](../resources/fido2authenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="00317-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="00317-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="00317-106">Permissions</span></span>
<span data-ttu-id="00317-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00317-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00317-109">Permission type</span></span>|<span data-ttu-id="00317-110">Permissões atuando por si mesmo (do mais para o menos privilegiado)</span><span class="sxs-lookup"><span data-stu-id="00317-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="00317-111">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="00317-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="00317-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00317-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="00317-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00317-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="00317-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00317-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="00317-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00317-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00317-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00317-116">Not supported.</span></span> | <span data-ttu-id="00317-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00317-117">Not supported.</span></span> |
| <span data-ttu-id="00317-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00317-118">Application</span></span>                            | <span data-ttu-id="00317-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="00317-119">Not applicable.</span></span> | <span data-ttu-id="00317-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00317-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="00317-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="00317-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="00317-122">Administração global</span><span class="sxs-lookup"><span data-stu-id="00317-122">Global admin</span></span>
* <span data-ttu-id="00317-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="00317-123">Global reader</span></span>
* <span data-ttu-id="00317-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="00317-124">Privileged authentication admin</span></span>
* <span data-ttu-id="00317-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="00317-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="00317-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00317-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00317-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00317-127">Optional query parameters</span></span>
<span data-ttu-id="00317-128">Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00317-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00317-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00317-129">Request headers</span></span>
|<span data-ttu-id="00317-130">Nome</span><span class="sxs-lookup"><span data-stu-id="00317-130">Name</span></span>|<span data-ttu-id="00317-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="00317-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="00317-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="00317-132">Authorization</span></span>|<span data-ttu-id="00317-133">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="00317-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="00317-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00317-134">Request body</span></span>
<span data-ttu-id="00317-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00317-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00317-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="00317-136">Response</span></span>

<span data-ttu-id="00317-137">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00317-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00317-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00317-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00317-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00317-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="00317-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="00317-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```
# <a name="c"></a>[<span data-ttu-id="00317-141">C#</span><span class="sxs-lookup"><span data-stu-id="00317-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00317-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00317-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00317-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00317-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00317-144">Java</span><span class="sxs-lookup"><span data-stu-id="00317-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="00317-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="00317-145">Response</span></span>
<span data-ttu-id="00317-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="00317-146">The following is an example of the response.</span></span>

<span data-ttu-id="00317-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="00317-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

