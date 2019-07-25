---
title: List oauth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: b6ec733c73d281e64978b11ebdf3c43d9eb94378
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878909"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="e69d5-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="e69d5-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e69d5-104">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e69d5-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e69d5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e69d5-105">Permissions</span></span>

<span data-ttu-id="e69d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e69d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e69d5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e69d5-108">Permission type</span></span>      | <span data-ttu-id="e69d5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e69d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e69d5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e69d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e69d5-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e69d5-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e69d5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e69d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e69d5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e69d5-113">Not supported.</span></span>    |
|<span data-ttu-id="e69d5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e69d5-114">Application</span></span> | <span data-ttu-id="e69d5-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e69d5-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e69d5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e69d5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e69d5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e69d5-117">Optional query parameters</span></span>
<span data-ttu-id="e69d5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e69d5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e69d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e69d5-119">Request headers</span></span>
| <span data-ttu-id="e69d5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e69d5-120">Name</span></span> | <span data-ttu-id="e69d5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e69d5-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="e69d5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e69d5-122">Authorization</span></span>  | <span data-ttu-id="e69d5-123">string</span><span class="sxs-lookup"><span data-stu-id="e69d5-123">string</span></span>  | <span data-ttu-id="e69d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e69d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e69d5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e69d5-126">Request body</span></span>
<span data-ttu-id="e69d5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e69d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e69d5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69d5-128">Response</span></span>

<span data-ttu-id="e69d5-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e69d5-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e69d5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e69d5-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e69d5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e69d5-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e69d5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e69d5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e69d5-133">C#</span><span class="sxs-lookup"><span data-stu-id="e69d5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e69d5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e69d5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e69d5-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e69d5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e69d5-136">Java</span><span class="sxs-lookup"><span data-stu-id="e69d5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e69d5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69d5-137">Response</span></span>

<span data-ttu-id="e69d5-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e69d5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
