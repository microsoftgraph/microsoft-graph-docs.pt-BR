---
title: Listar oAuth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant, representando as autorizações de permissão delegadas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 76934b9d1c5ffc31cfe6f7a72e6e0234419e7280
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028487"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="7b1c1-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="7b1c1-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="7b1c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b1c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b1c1-105">Recupere uma lista de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) , representando as permissões delegadas que foram concedidas para que os aplicativos clientes acessem APIs em nome de usuários conectados.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b1c1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b1c1-106">Permissions</span></span>

<span data-ttu-id="7b1c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b1c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b1c1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b1c1-109">Permission type</span></span>      | <span data-ttu-id="7b1c1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b1c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b1c1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b1c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b1c1-112">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="7b1c1-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b1c1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b1c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b1c1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-114">Not supported.</span></span>    |
|<span data-ttu-id="7b1c1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b1c1-115">Application</span></span> | <span data-ttu-id="7b1c1-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b1c1-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b1c1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b1c1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b1c1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b1c1-118">Optional query parameters</span></span>

<span data-ttu-id="7b1c1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b1c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b1c1-120">Request headers</span></span>

| <span data-ttu-id="7b1c1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7b1c1-121">Name</span></span>          | <span data-ttu-id="7b1c1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b1c1-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7b1c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b1c1-123">Authorization</span></span> | <span data-ttu-id="7b1c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b1c1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b1c1-126">Request body</span></span>

<span data-ttu-id="7b1c1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b1c1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b1c1-128">Response</span></span>

<span data-ttu-id="7b1c1-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b1c1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b1c1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b1c1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b1c1-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7b1c1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b1c1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="7b1c1-133">C#</span><span class="sxs-lookup"><span data-stu-id="7b1c1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b1c1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b1c1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b1c1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b1c1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b1c1-136">Java</span><span class="sxs-lookup"><span data-stu-id="7b1c1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b1c1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b1c1-137">Response</span></span>

> <span data-ttu-id="7b1c1-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b1c1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

