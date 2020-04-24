---
title: Métodos de List
description: Recupere uma lista de objetos de método de autenticação.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32dbbe0c87fbaaf19e93f434949408b3fea73523
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805919"
---
# <a name="list-methods"></a><span data-ttu-id="3dfac-103">Métodos de List</span><span class="sxs-lookup"><span data-stu-id="3dfac-103">List methods</span></span>

<span data-ttu-id="3dfac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dfac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dfac-105">Recupere uma lista de objetos de [método de autenticação](../resources/authenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="3dfac-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span> <span data-ttu-id="3dfac-106">Atualmente, apenas o [método de autenticação por telefone](../resources/phoneauthenticationmethod.md) e os objetos de método de autenticação de [senha](../resources/passwordauthenticationmethod.md) são retornados.</span><span class="sxs-lookup"><span data-stu-id="3dfac-106">Currently only [phone authentication method](../resources/phoneauthenticationmethod.md) and [password authentication method](../resources/passwordauthenticationmethod.md) objects are returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dfac-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dfac-107">Permissions</span></span>

<span data-ttu-id="3dfac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dfac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dfac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dfac-110">Permission type</span></span>                        | <span data-ttu-id="3dfac-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dfac-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="3dfac-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dfac-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="3dfac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dfac-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dfac-114">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3dfac-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="3dfac-115">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3dfac-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="3dfac-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dfac-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dfac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfac-117">Not supported.</span></span> | <span data-ttu-id="3dfac-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfac-118">Not supported.</span></span> |
| <span data-ttu-id="3dfac-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dfac-119">Application</span></span>                            | <span data-ttu-id="3dfac-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfac-120">Not supported.</span></span> | <span data-ttu-id="3dfac-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfac-121">Not supported.</span></span> |

<span data-ttu-id="3dfac-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="3dfac-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="3dfac-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3dfac-123">Global admin</span></span>
* <span data-ttu-id="3dfac-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="3dfac-124">Global reader</span></span>
* <span data-ttu-id="3dfac-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="3dfac-125">Privileged authentication admin</span></span>
* <span data-ttu-id="3dfac-126">Administrador de autenticação (apenas Ver os números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="3dfac-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="3dfac-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfac-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3dfac-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3dfac-128">Optional query parameters</span></span>

<span data-ttu-id="3dfac-129">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfac-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dfac-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfac-130">Request headers</span></span>

| <span data-ttu-id="3dfac-131">Nome</span><span class="sxs-lookup"><span data-stu-id="3dfac-131">Name</span></span>      |<span data-ttu-id="3dfac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dfac-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3dfac-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dfac-133">Authorization</span></span> | <span data-ttu-id="3dfac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dfac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dfac-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfac-136">Request body</span></span>

<span data-ttu-id="3dfac-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3dfac-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dfac-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dfac-138">Response</span></span>

<span data-ttu-id="3dfac-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [AuthenticationMethod](../resources/authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfac-139">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3dfac-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3dfac-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3dfac-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfac-141">Request</span></span>

<span data-ttu-id="3dfac-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dfac-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3dfac-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfac-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="3dfac-144">C#</span><span class="sxs-lookup"><span data-stu-id="3dfac-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dfac-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dfac-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dfac-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dfac-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3dfac-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dfac-147">Response</span></span>

<span data-ttu-id="3dfac-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfac-148">The following is an example of the response.</span></span>

> <span data-ttu-id="3dfac-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dfac-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
