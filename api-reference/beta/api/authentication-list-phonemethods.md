---
title: Listar phoneMethods
description: Recupere uma lista de objetos do método de autenticação de telefone.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5decfae13c3a8a53c90d94a61ecf0584d1b9da63
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047977"
---
# <a name="list-phonemethods"></a><span data-ttu-id="dfed5-103">Listar phoneMethods</span><span class="sxs-lookup"><span data-stu-id="dfed5-103">List phoneMethods</span></span>

<span data-ttu-id="dfed5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfed5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfed5-105">Recupere uma lista de objetos [do método de autenticação de](../resources/phoneauthenticationmethod.md) telefone.</span><span class="sxs-lookup"><span data-stu-id="dfed5-105">Retrieve a list of [phone authentication method](../resources/phoneauthenticationmethod.md) objects.</span></span> <span data-ttu-id="dfed5-106">Isso retornará até três objetos, pois um usuário pode ter até três telefones para autenticação.</span><span class="sxs-lookup"><span data-stu-id="dfed5-106">This will return up to three objects, as a user can have up to three phones usable for authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfed5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfed5-107">Permissions</span></span>

<span data-ttu-id="dfed5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfed5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfed5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfed5-110">Permission type</span></span>                        | <span data-ttu-id="dfed5-111">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="dfed5-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="dfed5-112">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="dfed5-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="dfed5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfed5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfed5-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfed5-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="dfed5-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfed5-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="dfed5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfed5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfed5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfed5-117">Not supported.</span></span> | <span data-ttu-id="dfed5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfed5-118">Not supported.</span></span> |
| <span data-ttu-id="dfed5-119">Application</span><span class="sxs-lookup"><span data-stu-id="dfed5-119">Application</span></span>                            | <span data-ttu-id="dfed5-120">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="dfed5-120">Not applicable.</span></span> | <span data-ttu-id="dfed5-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfed5-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="dfed5-122">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="dfed5-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="dfed5-123">Administração global</span><span class="sxs-lookup"><span data-stu-id="dfed5-123">Global admin</span></span>
* <span data-ttu-id="dfed5-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="dfed5-124">Global reader</span></span>
* <span data-ttu-id="dfed5-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="dfed5-125">Privileged authentication admin</span></span>
* <span data-ttu-id="dfed5-126">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="dfed5-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="dfed5-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfed5-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods
GET /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfed5-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfed5-128">Optional query parameters</span></span>

<span data-ttu-id="dfed5-129">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfed5-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfed5-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfed5-130">Request headers</span></span>

| <span data-ttu-id="dfed5-131">Nome</span><span class="sxs-lookup"><span data-stu-id="dfed5-131">Name</span></span>      |<span data-ttu-id="dfed5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfed5-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfed5-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfed5-133">Authorization</span></span> | <span data-ttu-id="dfed5-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="dfed5-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfed5-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfed5-135">Request body</span></span>

<span data-ttu-id="dfed5-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfed5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfed5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfed5-137">Response</span></span>

<span data-ttu-id="dfed5-138">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfed5-138">If successful, this method returns a `200 OK` response code and a collection of [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfed5-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfed5-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfed5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfed5-140">Request</span></span>

<span data-ttu-id="dfed5-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfed5-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfed5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfed5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phonemethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods
```
# <a name="c"></a>[<span data-ttu-id="dfed5-143">C#</span><span class="sxs-lookup"><span data-stu-id="dfed5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phonemethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfed5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfed5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phonemethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfed5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfed5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phonemethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfed5-146">Java</span><span class="sxs-lookup"><span data-stu-id="dfed5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phonemethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dfed5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfed5-147">Response</span></span>

<span data-ttu-id="dfed5-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfed5-148">The following is an example of the response.</span></span>

> <span data-ttu-id="dfed5-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dfed5-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "phoneNumber": "+1 2065555555",
      "phoneType": "mobile",
      "smsSignInState": "ready",
      "id": "3179e48a-750b-4051-897c-87b9720928f7"
    },
    {
      "phoneNumber": "+1 2065555556",
      "phoneType": "alternateMobile",
      "smsSignInState": "notSupported",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41"
    },
    {
      "phoneNumber": "+1 2065555557",
      "phoneType": "office",
      "smsSignInState": "notSupported",
      "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List phoneMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
