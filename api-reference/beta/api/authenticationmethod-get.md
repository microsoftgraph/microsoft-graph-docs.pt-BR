---
title: Obter authenticationMethod
description: Recupere as propriedades e os relacionamentos de um objeto authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 79921189e0c365d89d2c640f2e3404dadea45c06
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805716"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="ecc21-103">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ecc21-103">Get authenticationMethod</span></span>

<span data-ttu-id="ecc21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecc21-105">Recupere as propriedades e os relacionamentos de um objeto [AuthenticationMethod](../resources/authenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="ecc21-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc21-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecc21-106">Permissions</span></span>

<span data-ttu-id="ecc21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecc21-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecc21-109">Permission type</span></span>                        | <span data-ttu-id="ecc21-110">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecc21-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="ecc21-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecc21-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ecc21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecc21-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecc21-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ecc21-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="ecc21-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ecc21-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ecc21-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecc21-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecc21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecc21-116">Not supported.</span></span> | <span data-ttu-id="ecc21-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecc21-117">Not supported.</span></span> |
| <span data-ttu-id="ecc21-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecc21-118">Application</span></span>                            | <span data-ttu-id="ecc21-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecc21-119">Not supported.</span></span> | <span data-ttu-id="ecc21-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecc21-120">Not supported.</span></span> |

<span data-ttu-id="ecc21-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="ecc21-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="ecc21-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ecc21-122">Global admin</span></span>
* <span data-ttu-id="ecc21-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="ecc21-123">Global reader</span></span>
* <span data-ttu-id="ecc21-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="ecc21-124">Privileged authentication admin</span></span>
* <span data-ttu-id="ecc21-125">Administrador de autenticação (apenas Ver os números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="ecc21-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ecc21-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc21-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecc21-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecc21-127">Optional query parameters</span></span>

<span data-ttu-id="ecc21-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecc21-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecc21-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecc21-129">Request headers</span></span>

| <span data-ttu-id="ecc21-130">Nome</span><span class="sxs-lookup"><span data-stu-id="ecc21-130">Name</span></span>      |<span data-ttu-id="ecc21-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc21-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecc21-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecc21-132">Authorization</span></span> | <span data-ttu-id="ecc21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecc21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecc21-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecc21-135">Request body</span></span>

<span data-ttu-id="ecc21-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecc21-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc21-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecc21-137">Response</span></span>

<span data-ttu-id="ecc21-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [AuthenticationMethod](../resources/authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecc21-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecc21-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ecc21-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecc21-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecc21-140">Request</span></span>

<span data-ttu-id="ecc21-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecc21-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ecc21-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc21-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="ecc21-143">C#</span><span class="sxs-lookup"><span data-stu-id="ecc21-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecc21-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecc21-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecc21-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecc21-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecc21-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecc21-146">Response</span></span>

<span data-ttu-id="ecc21-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ecc21-147">The following is an example of the response.</span></span>

> <span data-ttu-id="ecc21-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecc21-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
