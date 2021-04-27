---
title: Obter um oAuth2PermissionGrant
description: Recupere as propriedades e as relações de oAuth2PermissionGrant único, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 05a21be27e0df9c408134556b38aa509b1881350
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038359"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="6aff7-103">Obter uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="6aff7-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="6aff7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aff7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6aff7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aff7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aff7-106">Recupere as propriedades de um [único oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="6aff7-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="6aff7-107">Um **oAuth2PermissionGrant** representa permissões delegadas que foram concedidas a um aplicativo cliente para acessar uma API em nome de um usuário interno.</span><span class="sxs-lookup"><span data-stu-id="6aff7-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aff7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6aff7-108">Permissions</span></span>

<span data-ttu-id="6aff7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aff7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aff7-111">Permission type</span></span>      | <span data-ttu-id="6aff7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6aff7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aff7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aff7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6aff7-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6aff7-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6aff7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aff7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aff7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aff7-116">Not supported.</span></span>    |
|<span data-ttu-id="6aff7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aff7-117">Application</span></span> | <span data-ttu-id="6aff7-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aff7-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aff7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aff7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6aff7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6aff7-120">Optional query parameters</span></span>

<span data-ttu-id="6aff7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6aff7-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6aff7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aff7-122">Request headers</span></span>

| <span data-ttu-id="6aff7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6aff7-123">Name</span></span>       | <span data-ttu-id="6aff7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aff7-124">Type</span></span> | <span data-ttu-id="6aff7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aff7-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6aff7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aff7-126">Authorization</span></span>  | <span data-ttu-id="6aff7-127">string</span><span class="sxs-lookup"><span data-stu-id="6aff7-127">string</span></span>  | <span data-ttu-id="6aff7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aff7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6aff7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aff7-130">Request body</span></span>

<span data-ttu-id="6aff7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6aff7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aff7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aff7-132">Response</span></span>

<span data-ttu-id="6aff7-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aff7-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aff7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aff7-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aff7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aff7-135">Request</span></span>

<span data-ttu-id="6aff7-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aff7-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6aff7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6aff7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="6aff7-138">C#</span><span class="sxs-lookup"><span data-stu-id="6aff7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6aff7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6aff7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6aff7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6aff7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6aff7-141">Java</span><span class="sxs-lookup"><span data-stu-id="6aff7-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6aff7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aff7-142">Response</span></span>

<span data-ttu-id="6aff7-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aff7-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="6aff7-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6aff7-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


