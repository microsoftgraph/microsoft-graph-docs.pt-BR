---
title: Obter fido2AuthenticationMethod
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4b5bad06b344db8355b1c73c7bf7886517795027
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959226"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="88cc5-103">Obter fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88cc5-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="88cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88cc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88cc5-105">Recupere o único objeto do método de autenticação de chave de segurança [FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="88cc5-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88cc5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88cc5-106">Permissions</span></span>
<span data-ttu-id="88cc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88cc5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88cc5-109">Permission type</span></span>|<span data-ttu-id="88cc5-110">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="88cc5-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="88cc5-111">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="88cc5-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="88cc5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88cc5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="88cc5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88cc5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="88cc5-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88cc5-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="88cc5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88cc5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88cc5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88cc5-116">Not supported.</span></span> | <span data-ttu-id="88cc5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88cc5-117">Not supported.</span></span> |
| <span data-ttu-id="88cc5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88cc5-118">Application</span></span>                            | <span data-ttu-id="88cc5-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="88cc5-119">Not applicable.</span></span> | <span data-ttu-id="88cc5-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88cc5-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="88cc5-121">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="88cc5-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="88cc5-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="88cc5-122">Global admin</span></span>
* <span data-ttu-id="88cc5-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="88cc5-123">Global reader</span></span>
* <span data-ttu-id="88cc5-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="88cc5-124">Privileged authentication admin</span></span>
* <span data-ttu-id="88cc5-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="88cc5-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="88cc5-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88cc5-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods/{id}
GET /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="88cc5-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88cc5-127">Request headers</span></span>
|<span data-ttu-id="88cc5-128">Nome</span><span class="sxs-lookup"><span data-stu-id="88cc5-128">Name</span></span>|<span data-ttu-id="88cc5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="88cc5-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88cc5-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="88cc5-130">Authorization</span></span>|<span data-ttu-id="88cc5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88cc5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88cc5-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88cc5-133">Request body</span></span>
<span data-ttu-id="88cc5-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88cc5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88cc5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="88cc5-135">Response</span></span>

<span data-ttu-id="88cc5-136">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88cc5-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88cc5-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="88cc5-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88cc5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88cc5-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88cc5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="88cc5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2
```
# <a name="c"></a>[<span data-ttu-id="88cc5-140">C#</span><span class="sxs-lookup"><span data-stu-id="88cc5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88cc5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88cc5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88cc5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88cc5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88cc5-143">Java</span><span class="sxs-lookup"><span data-stu-id="88cc5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88cc5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="88cc5-144">Response</span></span>
<span data-ttu-id="88cc5-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88cc5-145">The following is an example of the response.</span></span>

<span data-ttu-id="88cc5-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="88cc5-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

