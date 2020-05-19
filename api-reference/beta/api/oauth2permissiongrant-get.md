---
title: Obter um oAuth2PermissionGrant
description: Recupere as propriedades e os relacionamentos de um único oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ccc7fd1ab8ce060eea46a3bbb7db079a06ec9b28
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290199"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="d1308-103">Obter uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="d1308-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="d1308-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1308-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1308-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1308-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1308-106">Recupere as propriedades de um único [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="d1308-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="d1308-107">Um **oAuth2PermissionGrant** representa permissões delegadas que foram concedidas para um aplicativo cliente acessar uma API em nome de um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d1308-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1308-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1308-108">Permissions</span></span>

<span data-ttu-id="d1308-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1308-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1308-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1308-111">Permission type</span></span>      | <span data-ttu-id="d1308-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1308-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1308-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1308-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d1308-114">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="d1308-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1308-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1308-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1308-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1308-116">Not supported.</span></span>    |
|<span data-ttu-id="d1308-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1308-117">Application</span></span> | <span data-ttu-id="d1308-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1308-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1308-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1308-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1308-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1308-120">Optional query parameters</span></span>

<span data-ttu-id="d1308-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1308-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1308-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1308-122">Request headers</span></span>

| <span data-ttu-id="d1308-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d1308-123">Name</span></span>       | <span data-ttu-id="d1308-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1308-124">Type</span></span> | <span data-ttu-id="d1308-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1308-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d1308-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1308-126">Authorization</span></span>  | <span data-ttu-id="d1308-127">string</span><span class="sxs-lookup"><span data-stu-id="d1308-127">string</span></span>  | <span data-ttu-id="d1308-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1308-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1308-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1308-130">Request body</span></span>

<span data-ttu-id="d1308-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1308-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1308-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1308-132">Response</span></span>

<span data-ttu-id="d1308-133">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1308-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1308-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1308-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1308-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1308-135">Request</span></span>

<span data-ttu-id="d1308-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1308-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1308-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1308-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="d1308-138">C#</span><span class="sxs-lookup"><span data-stu-id="d1308-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1308-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1308-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1308-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1308-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d1308-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1308-141">Response</span></span>

<span data-ttu-id="d1308-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1308-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="d1308-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1308-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
