---
title: Obter fido2AuthenticationMethod
description: Leia as propriedades e as relações de um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ecde3c3432064cf01636e3a8d267773920fcf1f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872146"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="5d41e-103">Obter fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5d41e-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="5d41e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d41e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d41e-105">Recupere o único objeto de método de autenticação de [chave de segurança FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="5d41e-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d41e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d41e-106">Permissions</span></span>
<span data-ttu-id="5d41e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d41e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d41e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d41e-109">Permission type</span></span>|<span data-ttu-id="5d41e-110">Permissões atuando por si mesmo (do menos para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="5d41e-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="5d41e-111">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="5d41e-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="5d41e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d41e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d41e-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d41e-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="5d41e-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d41e-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="5d41e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d41e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d41e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d41e-116">Not supported.</span></span> | <span data-ttu-id="5d41e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d41e-117">Not supported.</span></span> |
| <span data-ttu-id="5d41e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d41e-118">Application</span></span>                            | <span data-ttu-id="5d41e-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="5d41e-119">Not applicable.</span></span> | <span data-ttu-id="5d41e-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d41e-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="5d41e-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="5d41e-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5d41e-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5d41e-122">Global admin</span></span>
* <span data-ttu-id="5d41e-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="5d41e-123">Global reader</span></span>
* <span data-ttu-id="5d41e-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="5d41e-124">Privileged authentication admin</span></span>
* <span data-ttu-id="5d41e-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="5d41e-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5d41e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d41e-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5d41e-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d41e-127">Request headers</span></span>
|<span data-ttu-id="5d41e-128">Nome</span><span class="sxs-lookup"><span data-stu-id="5d41e-128">Name</span></span>|<span data-ttu-id="5d41e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d41e-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d41e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d41e-130">Authorization</span></span>|<span data-ttu-id="5d41e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d41e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d41e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d41e-133">Request body</span></span>
<span data-ttu-id="5d41e-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d41e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d41e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d41e-135">Response</span></span>

<span data-ttu-id="5d41e-136">Se bem-sucedido, este método retorna um código de resposta e o objeto `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d41e-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d41e-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5d41e-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d41e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d41e-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d41e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d41e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```
# <a name="c"></a>[<span data-ttu-id="5d41e-140">C#</span><span class="sxs-lookup"><span data-stu-id="5d41e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d41e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d41e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d41e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d41e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d41e-143">Java</span><span class="sxs-lookup"><span data-stu-id="5d41e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5d41e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d41e-144">Response</span></span>
<span data-ttu-id="5d41e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d41e-145">The following is an example of the response.</span></span>

<span data-ttu-id="5d41e-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d41e-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

