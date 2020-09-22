---
title: Listar passwordMethods
description: Recupere uma lista de objetos passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da71ed2ff778ac80dad1a6949622b8b4773f1106
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991667"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="bf359-103">Listar passwordMethods</span><span class="sxs-lookup"><span data-stu-id="bf359-103">List passwordMethods</span></span>

<span data-ttu-id="bf359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf359-105">Recupere uma lista de objetos de [método de autenticação de senha](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="bf359-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="bf359-106">Isso retornará exatamente um objeto, pois um usuário pode ter exatamente uma senha.</span><span class="sxs-lookup"><span data-stu-id="bf359-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf359-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf359-107">Permissions</span></span>

<span data-ttu-id="bf359-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf359-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf359-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf359-110">Permission type</span></span>                        | <span data-ttu-id="bf359-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf359-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="bf359-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf359-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="bf359-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf359-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf359-114">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bf359-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="bf359-115">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bf359-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="bf359-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf359-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf359-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf359-117">Not supported.</span></span> | <span data-ttu-id="bf359-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf359-118">Not supported.</span></span> |
| <span data-ttu-id="bf359-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf359-119">Application</span></span>                            | <span data-ttu-id="bf359-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf359-120">Not supported.</span></span> | <span data-ttu-id="bf359-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf359-121">Not supported.</span></span> |

<span data-ttu-id="bf359-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="bf359-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="bf359-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bf359-123">Global admin</span></span>
* <span data-ttu-id="bf359-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="bf359-124">Global reader</span></span>
* <span data-ttu-id="bf359-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="bf359-125">Privileged authentication admin</span></span>
* <span data-ttu-id="bf359-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="bf359-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="bf359-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf359-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf359-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bf359-128">Optional query parameters</span></span>

<span data-ttu-id="bf359-129">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bf359-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf359-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf359-130">Request headers</span></span>

| <span data-ttu-id="bf359-131">Nome</span><span class="sxs-lookup"><span data-stu-id="bf359-131">Name</span></span>      |<span data-ttu-id="bf359-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf359-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf359-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf359-133">Authorization</span></span> | <span data-ttu-id="bf359-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="bf359-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf359-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf359-135">Request body</span></span>

<span data-ttu-id="bf359-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf359-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf359-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf359-137">Response</span></span>

<span data-ttu-id="bf359-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf359-138">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf359-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bf359-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf359-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf359-140">Request</span></span>

<span data-ttu-id="bf359-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf359-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf359-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf359-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="bf359-143">C#</span><span class="sxs-lookup"><span data-stu-id="bf359-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf359-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf359-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf359-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf359-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf359-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf359-146">Response</span></span>

<span data-ttu-id="bf359-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bf359-147">The following is an example of the response.</span></span>

> <span data-ttu-id="bf359-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf359-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List passwordMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


