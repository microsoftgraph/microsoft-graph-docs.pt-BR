---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b81fb9f05787bce51b0de55e1993db60ecfa6d8
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721247"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="cd2db-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="cd2db-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="cd2db-104">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="cd2db-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd2db-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd2db-105">Permissions</span></span>
<span data-ttu-id="cd2db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd2db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd2db-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd2db-108">Permission type</span></span>      | <span data-ttu-id="cd2db-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd2db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd2db-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd2db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd2db-111">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="cd2db-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd2db-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd2db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd2db-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd2db-113">Not supported.</span></span>    |
|<span data-ttu-id="cd2db-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd2db-114">Application</span></span> | <span data-ttu-id="cd2db-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cd2db-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd2db-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd2db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd2db-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cd2db-117">Optional query parameters</span></span>
<span data-ttu-id="cd2db-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="cd2db-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd2db-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd2db-119">Request headers</span></span>
| <span data-ttu-id="cd2db-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cd2db-120">Name</span></span>       | <span data-ttu-id="cd2db-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2db-121">Type</span></span> | <span data-ttu-id="cd2db-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2db-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd2db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd2db-123">Authorization</span></span>  | <span data-ttu-id="cd2db-124">string</span><span class="sxs-lookup"><span data-stu-id="cd2db-124">string</span></span>  | <span data-ttu-id="cd2db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd2db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd2db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd2db-127">Request body</span></span>
<span data-ttu-id="cd2db-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd2db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd2db-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd2db-129">Response</span></span>

<span data-ttu-id="cd2db-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd2db-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd2db-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd2db-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd2db-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd2db-132">Request</span></span>
<span data-ttu-id="cd2db-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd2db-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cd2db-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd2db-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd2db-135">C#</span><span class="sxs-lookup"><span data-stu-id="cd2db-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd2db-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd2db-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd2db-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cd2db-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cd2db-138">Java</span><span class="sxs-lookup"><span data-stu-id="cd2db-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cd2db-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd2db-139">Response</span></span>
<span data-ttu-id="cd2db-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd2db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
