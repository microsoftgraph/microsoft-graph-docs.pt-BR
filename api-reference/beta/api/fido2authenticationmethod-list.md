---
title: Listar fido2AuthenticationMethod
description: Recupere uma lista dos objetos fido2AuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad8a3d3c90299dcf72bb5103059420a4db4ec514
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458863"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="b4e2f-103">Listar fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b4e2f-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="b4e2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4e2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4e2f-105">Recupere uma lista de objetos de [método de autenticação de chave de segurança FIDO2](../resources/fido2authenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4e2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4e2f-106">Permissions</span></span>
<span data-ttu-id="b4e2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4e2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4e2f-109">Permission type</span></span>|<span data-ttu-id="b4e2f-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4e2f-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="b4e2f-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4e2f-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="b4e2f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4e2f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4e2f-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b4e2f-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="b4e2f-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b4e2f-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="b4e2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4e2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4e2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-116">Not supported.</span></span>|<span data-ttu-id="b4e2f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-117">Not supported.</span></span>
|<span data-ttu-id="b4e2f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4e2f-118">Application</span></span>|<span data-ttu-id="b4e2f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-119">Not supported.</span></span>|<span data-ttu-id="b4e2f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-120">Not supported.</span></span>

<span data-ttu-id="b4e2f-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="b4e2f-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b4e2f-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b4e2f-122">Global admin</span></span>
* <span data-ttu-id="b4e2f-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="b4e2f-123">Global reader</span></span>
* <span data-ttu-id="b4e2f-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="b4e2f-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b4e2f-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="b4e2f-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b4e2f-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4e2f-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4e2f-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b4e2f-127">Optional query parameters</span></span>
<span data-ttu-id="b4e2f-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4e2f-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4e2f-129">Request headers</span></span>
|<span data-ttu-id="b4e2f-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b4e2f-130">Name</span></span>|<span data-ttu-id="b4e2f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4e2f-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4e2f-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4e2f-132">Authorization</span></span>|<span data-ttu-id="b4e2f-133">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b4e2f-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4e2f-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4e2f-134">Request body</span></span>
<span data-ttu-id="b4e2f-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4e2f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4e2f-136">Response</span></span>

<span data-ttu-id="b4e2f-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4e2f-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b4e2f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4e2f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4e2f-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b4e2f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4e2f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```
# <a name="c"></a>[<span data-ttu-id="b4e2f-141">C#</span><span class="sxs-lookup"><span data-stu-id="b4e2f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4e2f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4e2f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4e2f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4e2f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b4e2f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4e2f-144">Response</span></span>
<span data-ttu-id="b4e2f-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-145">The following is an example of the response.</span></span>

<span data-ttu-id="b4e2f-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b4e2f-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

