---
title: 'servicePrincipalName: listar oAuth2Permissiongrants'
description: Recupere uma lista de objetos oAuth2Permissiongrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f52216a7bf50dc346099367c273075768f7cbe70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991363"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="86fd2-103">servicePrincipalName: listar oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="86fd2-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86fd2-104">Recupere uma lista de objetos oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="86fd2-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="86fd2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86fd2-105">Permissions</span></span>
<span data-ttu-id="86fd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86fd2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86fd2-108">Permission type</span></span>      | <span data-ttu-id="86fd2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86fd2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86fd2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86fd2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86fd2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86fd2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86fd2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86fd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86fd2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86fd2-113">Not supported.</span></span>    |
|<span data-ttu-id="86fd2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86fd2-114">Application</span></span> | <span data-ttu-id="86fd2-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86fd2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86fd2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86fd2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86fd2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86fd2-117">Optional query parameters</span></span>
<span data-ttu-id="86fd2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86fd2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86fd2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86fd2-119">Request headers</span></span>
| <span data-ttu-id="86fd2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="86fd2-120">Name</span></span>       | <span data-ttu-id="86fd2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="86fd2-121">Type</span></span> | <span data-ttu-id="86fd2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="86fd2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="86fd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86fd2-123">Authorization</span></span>  | <span data-ttu-id="86fd2-124">string</span><span class="sxs-lookup"><span data-stu-id="86fd2-124">string</span></span>  | <span data-ttu-id="86fd2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86fd2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86fd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86fd2-127">Request body</span></span>
<span data-ttu-id="86fd2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86fd2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86fd2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="86fd2-129">Response</span></span>

<span data-ttu-id="86fd2-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86fd2-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86fd2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86fd2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86fd2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86fd2-132">Request</span></span>
<span data-ttu-id="86fd2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86fd2-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86fd2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="86fd2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86fd2-135">C#</span><span class="sxs-lookup"><span data-stu-id="86fd2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86fd2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="86fd2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86fd2-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="86fd2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="86fd2-138">Java</span><span class="sxs-lookup"><span data-stu-id="86fd2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86fd2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="86fd2-139">Response</span></span>
<span data-ttu-id="86fd2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86fd2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
