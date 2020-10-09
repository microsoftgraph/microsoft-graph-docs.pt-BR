---
title: Obter phoneAuthenticationMethod
description: Recupere um único objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8aedb4e643bcffa727ddbe3e0b4299fb917389ee
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402636"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="3bee5-103">Obter phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3bee5-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="3bee5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bee5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bee5-105">Recupere um único objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="3bee5-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bee5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bee5-106">Permissions</span></span>

<span data-ttu-id="3bee5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bee5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bee5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bee5-109">Permission type</span></span>                        | <span data-ttu-id="3bee5-110">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bee5-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="3bee5-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bee5-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="3bee5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bee5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bee5-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3bee5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="3bee5-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3bee5-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="3bee5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bee5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bee5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bee5-116">Not supported.</span></span> | <span data-ttu-id="3bee5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bee5-117">Not supported.</span></span> |
| <span data-ttu-id="3bee5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bee5-118">Application</span></span>                            | <span data-ttu-id="3bee5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bee5-119">Not supported.</span></span> | <span data-ttu-id="3bee5-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bee5-120">Not supported.</span></span> |

<span data-ttu-id="3bee5-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="3bee5-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="3bee5-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3bee5-122">Global admin</span></span>
* <span data-ttu-id="3bee5-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="3bee5-123">Global reader</span></span>
* <span data-ttu-id="3bee5-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="3bee5-124">Privileged authentication admin</span></span>
* <span data-ttu-id="3bee5-125">Administrador de autenticação (apenas Ver os números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="3bee5-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="3bee5-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bee5-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id}/authentication/phoneMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bee5-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bee5-127">Optional query parameters</span></span>

<span data-ttu-id="3bee5-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bee5-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bee5-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bee5-129">Request headers</span></span>

| <span data-ttu-id="3bee5-130">Nome</span><span class="sxs-lookup"><span data-stu-id="3bee5-130">Name</span></span>      |<span data-ttu-id="3bee5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bee5-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3bee5-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bee5-132">Authorization</span></span> | <span data-ttu-id="3bee5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bee5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bee5-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bee5-135">Request body</span></span>

<span data-ttu-id="3bee5-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bee5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bee5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bee5-137">Response</span></span>

<span data-ttu-id="3bee5-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bee5-138">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3bee5-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3bee5-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3bee5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bee5-140">Request</span></span>

<span data-ttu-id="3bee5-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bee5-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3bee5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bee5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="3bee5-143">C#</span><span class="sxs-lookup"><span data-stu-id="3bee5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bee5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bee5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bee5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bee5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3bee5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bee5-146">Response</span></span>

<span data-ttu-id="3bee5-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3bee5-147">The following is an example of the response.</span></span>

> <span data-ttu-id="3bee5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bee5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->