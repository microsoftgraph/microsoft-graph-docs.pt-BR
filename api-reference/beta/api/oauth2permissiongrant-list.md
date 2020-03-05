---
title: List oauth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf36b48d2f0a1aa5478a78ad211348a815e0d790
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456616"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="b0ba1-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="b0ba1-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="b0ba1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0ba1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ba1-105">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-105">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0ba1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0ba1-106">Permissions</span></span>

<span data-ttu-id="b0ba1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0ba1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0ba1-109">Permission type</span></span>      | <span data-ttu-id="b0ba1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0ba1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ba1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0ba1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ba1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0ba1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0ba1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0ba1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ba1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-114">Not supported.</span></span>    |
|<span data-ttu-id="b0ba1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0ba1-115">Application</span></span> | <span data-ttu-id="b0ba1-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0ba1-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ba1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0ba1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0ba1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0ba1-118">Optional query parameters</span></span>
<span data-ttu-id="b0ba1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0ba1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0ba1-120">Request headers</span></span>
| <span data-ttu-id="b0ba1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b0ba1-121">Name</span></span> | <span data-ttu-id="b0ba1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ba1-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b0ba1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0ba1-123">Authorization</span></span>  | <span data-ttu-id="b0ba1-124">string</span><span class="sxs-lookup"><span data-stu-id="b0ba1-124">string</span></span>  | <span data-ttu-id="b0ba1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0ba1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0ba1-127">Request body</span></span>
<span data-ttu-id="b0ba1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0ba1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0ba1-129">Response</span></span>

<span data-ttu-id="b0ba1-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0ba1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0ba1-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0ba1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0ba1-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b0ba1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0ba1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="b0ba1-134">C#</span><span class="sxs-lookup"><span data-stu-id="b0ba1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0ba1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0ba1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0ba1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0ba1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0ba1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0ba1-137">Response</span></span>

<span data-ttu-id="b0ba1-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0ba1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
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
