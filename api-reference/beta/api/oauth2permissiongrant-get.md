---
title: Obter oAuth2Permissiongrant
description: Recupere as propriedades e os relacionamentos do objeto oAuth2Permissiongrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 760e73e0bedec62b8166139d3aa3e96615417577
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200317"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="86483-103">Obter oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="86483-103">Get oAuth2Permissiongrant</span></span>

<span data-ttu-id="86483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86483-105">Recupere as propriedades e os relacionamentos do objeto oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="86483-105">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86483-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86483-106">Permissions</span></span>
<span data-ttu-id="86483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="86483-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86483-109">Permission type</span></span>      | <span data-ttu-id="86483-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86483-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86483-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86483-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86483-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86483-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86483-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86483-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86483-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86483-114">Not supported.</span></span>    |
|<span data-ttu-id="86483-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86483-115">Application</span></span> | <span data-ttu-id="86483-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86483-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86483-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86483-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86483-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86483-118">Optional query parameters</span></span>
<span data-ttu-id="86483-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86483-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86483-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86483-120">Request headers</span></span>
| <span data-ttu-id="86483-121">Nome</span><span class="sxs-lookup"><span data-stu-id="86483-121">Name</span></span>       | <span data-ttu-id="86483-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="86483-122">Type</span></span> | <span data-ttu-id="86483-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="86483-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="86483-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="86483-124">Authorization</span></span>  | <span data-ttu-id="86483-125">string</span><span class="sxs-lookup"><span data-stu-id="86483-125">string</span></span>  | <span data-ttu-id="86483-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86483-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86483-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86483-128">Request body</span></span>
<span data-ttu-id="86483-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86483-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86483-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="86483-130">Response</span></span>

<span data-ttu-id="86483-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86483-131">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86483-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86483-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86483-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86483-133">Request</span></span>
<span data-ttu-id="86483-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86483-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86483-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="86483-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="86483-136">C#</span><span class="sxs-lookup"><span data-stu-id="86483-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86483-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86483-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86483-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86483-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86483-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="86483-139">Response</span></span>
<span data-ttu-id="86483-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86483-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
