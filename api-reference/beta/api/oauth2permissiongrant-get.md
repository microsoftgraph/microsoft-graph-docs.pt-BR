---
title: Obter um oAuth2PermissionGrant
description: Recupere as propriedades e as relações de oAuth2PermissionGrant único, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 4919e2e664ba3af1d3b74c8af9f7f5047c915a16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442368"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="5322f-103">Obter uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="5322f-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="5322f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5322f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5322f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5322f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5322f-106">Recupere as propriedades de um [único oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="5322f-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="5322f-107">Um **oAuth2PermissionGrant** representa permissões delegadas que foram concedidas a um aplicativo cliente para acessar uma API em nome de um usuário interno.</span><span class="sxs-lookup"><span data-stu-id="5322f-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5322f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5322f-108">Permissions</span></span>

<span data-ttu-id="5322f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5322f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5322f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5322f-111">Permission type</span></span>      | <span data-ttu-id="5322f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5322f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5322f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5322f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5322f-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5322f-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5322f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5322f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5322f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5322f-116">Not supported.</span></span>    |
|<span data-ttu-id="5322f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5322f-117">Application</span></span> | <span data-ttu-id="5322f-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5322f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5322f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5322f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5322f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5322f-120">Optional query parameters</span></span>

<span data-ttu-id="5322f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5322f-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5322f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5322f-122">Request headers</span></span>

| <span data-ttu-id="5322f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5322f-123">Name</span></span>       | <span data-ttu-id="5322f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5322f-124">Type</span></span> | <span data-ttu-id="5322f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5322f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5322f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5322f-126">Authorization</span></span>  | <span data-ttu-id="5322f-127">string</span><span class="sxs-lookup"><span data-stu-id="5322f-127">string</span></span>  | <span data-ttu-id="5322f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5322f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5322f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5322f-130">Request body</span></span>

<span data-ttu-id="5322f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5322f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5322f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5322f-132">Response</span></span>

<span data-ttu-id="5322f-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5322f-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5322f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5322f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="5322f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5322f-135">Request</span></span>

<span data-ttu-id="5322f-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5322f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5322f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5322f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="5322f-138">C#</span><span class="sxs-lookup"><span data-stu-id="5322f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5322f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5322f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5322f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5322f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5322f-141">Java</span><span class="sxs-lookup"><span data-stu-id="5322f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5322f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5322f-142">Response</span></span>

<span data-ttu-id="5322f-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5322f-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="5322f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5322f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


