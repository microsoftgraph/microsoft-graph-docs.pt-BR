---
title: Obter um oAuth2PermissionGrant
description: Recupere as propriedades e as relações de oAuth2PermissionGrant único, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 86e1bd2bbf03ac9304082bee44e5ed6e46ff00fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039325"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="40289-103">Obter uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="40289-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="40289-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40289-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40289-105">Recupere as propriedades de um [único oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="40289-105">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="40289-106">Um **oAuth2PermissionGrant** representa permissões delegadas que foram concedidas a um aplicativo cliente para acessar uma API em nome de um usuário interno.</span><span class="sxs-lookup"><span data-stu-id="40289-106">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="40289-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="40289-107">Permissions</span></span>

<span data-ttu-id="40289-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40289-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40289-110">Permission type</span></span>      | <span data-ttu-id="40289-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40289-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40289-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40289-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40289-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40289-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40289-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40289-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40289-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40289-115">Not supported.</span></span>    |
|<span data-ttu-id="40289-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40289-116">Application</span></span> | <span data-ttu-id="40289-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40289-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40289-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40289-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40289-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40289-119">Optional query parameters</span></span>

<span data-ttu-id="40289-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40289-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40289-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40289-121">Request headers</span></span>

| <span data-ttu-id="40289-122">Nome</span><span class="sxs-lookup"><span data-stu-id="40289-122">Name</span></span>       | <span data-ttu-id="40289-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="40289-123">Type</span></span> | <span data-ttu-id="40289-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="40289-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40289-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="40289-125">Authorization</span></span>  | <span data-ttu-id="40289-126">string</span><span class="sxs-lookup"><span data-stu-id="40289-126">string</span></span>  | <span data-ttu-id="40289-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40289-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40289-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40289-129">Request body</span></span>

<span data-ttu-id="40289-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40289-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40289-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40289-131">Response</span></span>

<span data-ttu-id="40289-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40289-132">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40289-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40289-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="40289-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40289-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="40289-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="40289-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="40289-136">C#</span><span class="sxs-lookup"><span data-stu-id="40289-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40289-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40289-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40289-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40289-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40289-139">Java</span><span class="sxs-lookup"><span data-stu-id="40289-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40289-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="40289-140">Response</span></span>

> <span data-ttu-id="40289-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40289-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "scope": "scope-value"
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

