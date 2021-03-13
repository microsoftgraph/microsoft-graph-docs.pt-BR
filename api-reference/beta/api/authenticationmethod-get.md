---
title: Obter authenticationMethod
description: Recupere as propriedades e as relações de um objeto authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 10495d9b66c63207ec1b1376efcb1796b9e4c9ad
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760025"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="be1d9-103">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="be1d9-103">Get authenticationMethod</span></span>

<span data-ttu-id="be1d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be1d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be1d9-105">Recupere as propriedades e as relações de um [objeto authenticationMethod.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="be1d9-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be1d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be1d9-106">Permissions</span></span>

<span data-ttu-id="be1d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be1d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be1d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be1d9-109">Permission type</span></span>                        | <span data-ttu-id="be1d9-110">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="be1d9-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="be1d9-111">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="be1d9-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="be1d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be1d9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="be1d9-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be1d9-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="be1d9-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be1d9-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="be1d9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be1d9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be1d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be1d9-116">Not supported.</span></span> | <span data-ttu-id="be1d9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be1d9-117">Not supported.</span></span> |
| <span data-ttu-id="be1d9-118">Application</span><span class="sxs-lookup"><span data-stu-id="be1d9-118">Application</span></span>                            | <span data-ttu-id="be1d9-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="be1d9-119">Not applicable.</span></span> | <span data-ttu-id="be1d9-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be1d9-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="be1d9-121">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="be1d9-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="be1d9-122">Administração global</span><span class="sxs-lookup"><span data-stu-id="be1d9-122">Global admin</span></span>
* <span data-ttu-id="be1d9-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="be1d9-123">Global reader</span></span>
* <span data-ttu-id="be1d9-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="be1d9-124">Privileged authentication admin</span></span>
* <span data-ttu-id="be1d9-125">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="be1d9-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="be1d9-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be1d9-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be1d9-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be1d9-127">Optional query parameters</span></span>

<span data-ttu-id="be1d9-128">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be1d9-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be1d9-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be1d9-129">Request headers</span></span>

| <span data-ttu-id="be1d9-130">Nome</span><span class="sxs-lookup"><span data-stu-id="be1d9-130">Name</span></span>      |<span data-ttu-id="be1d9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be1d9-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be1d9-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="be1d9-132">Authorization</span></span> | <span data-ttu-id="be1d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be1d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be1d9-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be1d9-135">Request body</span></span>

<span data-ttu-id="be1d9-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be1d9-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be1d9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="be1d9-137">Response</span></span>

<span data-ttu-id="be1d9-138">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [authenticationMethod](../resources/authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be1d9-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be1d9-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be1d9-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be1d9-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be1d9-140">Request</span></span>

<span data-ttu-id="be1d9-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be1d9-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be1d9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="be1d9-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="be1d9-143">C#</span><span class="sxs-lookup"><span data-stu-id="be1d9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be1d9-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be1d9-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be1d9-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be1d9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be1d9-146">Java</span><span class="sxs-lookup"><span data-stu-id="be1d9-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be1d9-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="be1d9-147">Response</span></span>

<span data-ttu-id="be1d9-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be1d9-148">The following is an example of the response.</span></span>

> <span data-ttu-id="be1d9-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be1d9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "3179e48a-750b-4051-897c-87b9720928f7",
  "phoneNumber": "+1 2065555555",
  "authenticationPhoneType": "mobile",
  "smsSignInState": "ready"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
