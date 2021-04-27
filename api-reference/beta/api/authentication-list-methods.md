---
title: Métodos de List
description: Recupere uma lista de objetos do método de autenticação.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 05606726178d2c1d2a2bb308f941810363e357c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047998"
---
# <a name="list-methods"></a><span data-ttu-id="61ea0-103">Métodos de List</span><span class="sxs-lookup"><span data-stu-id="61ea0-103">List methods</span></span>

<span data-ttu-id="61ea0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61ea0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61ea0-105">Recupere uma lista de objetos [do método de autenticação.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="61ea0-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="61ea0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61ea0-106">Permissions</span></span>

<span data-ttu-id="61ea0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="61ea0-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="61ea0-109">Permissions acting on self</span></span>

|<span data-ttu-id="61ea0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61ea0-110">Permission type</span></span>      | <span data-ttu-id="61ea0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61ea0-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="61ea0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61ea0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="61ea0-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61ea0-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="61ea0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61ea0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61ea0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ea0-115">Not supported.</span></span> |
| <span data-ttu-id="61ea0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61ea0-116">Application</span></span>                            | <span data-ttu-id="61ea0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ea0-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="61ea0-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="61ea0-118">Permissions acting on other users</span></span>

|<span data-ttu-id="61ea0-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61ea0-119">Permission type</span></span>      | <span data-ttu-id="61ea0-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61ea0-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="61ea0-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61ea0-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="61ea0-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61ea0-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="61ea0-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61ea0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61ea0-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ea0-124">Not supported.</span></span> |
| <span data-ttu-id="61ea0-125">Application</span><span class="sxs-lookup"><span data-stu-id="61ea0-125">Application</span></span>                            | <span data-ttu-id="61ea0-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61ea0-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="61ea0-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="61ea0-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="61ea0-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="61ea0-128">Global admin</span></span>
* <span data-ttu-id="61ea0-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="61ea0-129">Global reader</span></span>
* <span data-ttu-id="61ea0-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="61ea0-130">Privileged authentication admin</span></span>
* <span data-ttu-id="61ea0-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="61ea0-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="61ea0-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61ea0-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61ea0-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61ea0-133">Optional query parameters</span></span>

<span data-ttu-id="61ea0-134">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61ea0-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61ea0-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61ea0-135">Request headers</span></span>

| <span data-ttu-id="61ea0-136">Nome</span><span class="sxs-lookup"><span data-stu-id="61ea0-136">Name</span></span>      |<span data-ttu-id="61ea0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="61ea0-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61ea0-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="61ea0-138">Authorization</span></span> | <span data-ttu-id="61ea0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61ea0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61ea0-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61ea0-141">Request body</span></span>

<span data-ttu-id="61ea0-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61ea0-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61ea0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="61ea0-143">Response</span></span>

<span data-ttu-id="61ea0-144">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [authenticationMethod](../resources/authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61ea0-144">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61ea0-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61ea0-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61ea0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61ea0-146">Request</span></span>

<span data-ttu-id="61ea0-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61ea0-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61ea0-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="61ea0-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="61ea0-149">C#</span><span class="sxs-lookup"><span data-stu-id="61ea0-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61ea0-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61ea0-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61ea0-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61ea0-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61ea0-152">Java</span><span class="sxs-lookup"><span data-stu-id="61ea0-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-methods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61ea0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="61ea0-153">Response</span></span>

<span data-ttu-id="61ea0-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61ea0-154">The following is an example of the response.</span></span>

> <span data-ttu-id="61ea0-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="61ea0-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "odata.type": "#microsoft.graph.passwordAuthenticationMethod",
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "3179e48a-750b-4051-897c-87b9720928f7",
      "phoneNumber": "+1 2065555555",
      "authenticationPhoneType": "mobile",
      "smsSignInState": "ready"
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41",
      "phoneNumber": "+1 2065555556",
      "authenticationPhoneType": "alternateMobile",
      "smsSignInState": "notSupported"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
