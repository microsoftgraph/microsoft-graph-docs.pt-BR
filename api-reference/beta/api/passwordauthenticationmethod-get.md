---
title: Obter passwordAuthenticationMethod
description: Recupere as propriedades e os relacionamentos do objeto passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44506848052e07d0cfb006b68d6a6052e4863436
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973051"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="a00f2-103">Obter passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a00f2-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="a00f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a00f2-105">Recupere as propriedades e os relacionamentos de um objeto de [método de autenticação de senha](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="a00f2-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a00f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a00f2-106">Permissions</span></span>

<span data-ttu-id="a00f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a00f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a00f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a00f2-109">Permission type</span></span>                        | <span data-ttu-id="a00f2-110">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a00f2-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="a00f2-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a00f2-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a00f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a00f2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a00f2-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a00f2-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="a00f2-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a00f2-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a00f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a00f2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a00f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00f2-116">Not supported.</span></span> | <span data-ttu-id="a00f2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00f2-117">Not supported.</span></span> |
| <span data-ttu-id="a00f2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a00f2-118">Application</span></span>                            | <span data-ttu-id="a00f2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00f2-119">Not supported.</span></span> | <span data-ttu-id="a00f2-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00f2-120">Not supported.</span></span> |

<span data-ttu-id="a00f2-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="a00f2-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="a00f2-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a00f2-122">Global admin</span></span>
* <span data-ttu-id="a00f2-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="a00f2-123">Global reader</span></span>
* <span data-ttu-id="a00f2-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="a00f2-124">Privileged authentication admin</span></span>
* <span data-ttu-id="a00f2-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="a00f2-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="a00f2-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a00f2-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a00f2-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a00f2-127">Optional query parameters</span></span>

<span data-ttu-id="a00f2-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a00f2-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a00f2-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a00f2-129">Request headers</span></span>

| <span data-ttu-id="a00f2-130">Nome</span><span class="sxs-lookup"><span data-stu-id="a00f2-130">Name</span></span>      |<span data-ttu-id="a00f2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00f2-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a00f2-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="a00f2-132">Authorization</span></span> | <span data-ttu-id="a00f2-133">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a00f2-133">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a00f2-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a00f2-134">Request body</span></span>

<span data-ttu-id="a00f2-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a00f2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a00f2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00f2-136">Response</span></span>

<span data-ttu-id="a00f2-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a00f2-137">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a00f2-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a00f2-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a00f2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a00f2-139">Request</span></span>

<span data-ttu-id="a00f2-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a00f2-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a00f2-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a00f2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="a00f2-142">C#</span><span class="sxs-lookup"><span data-stu-id="a00f2-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a00f2-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a00f2-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a00f2-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a00f2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a00f2-145">Java</span><span class="sxs-lookup"><span data-stu-id="a00f2-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a00f2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00f2-146">Response</span></span>

<span data-ttu-id="a00f2-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a00f2-147">The following is an example of the response.</span></span>

> <span data-ttu-id="a00f2-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a00f2-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "28c10230-6103-485e-b985-444c60001490",
  "password": null,
  "creationDateTime": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get passwordAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
