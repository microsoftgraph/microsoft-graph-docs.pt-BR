---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac25dafd1209728de828f904a694f13c0b3990b2
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180855"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="578a3-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="578a3-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="578a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="578a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="578a3-105">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="578a3-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="578a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="578a3-106">Permissions</span></span>
<span data-ttu-id="578a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="578a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="578a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="578a3-109">Permission type</span></span>      | <span data-ttu-id="578a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="578a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="578a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="578a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="578a3-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="578a3-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="578a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="578a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="578a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="578a3-114">Not supported.</span></span>    |
|<span data-ttu-id="578a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="578a3-115">Application</span></span> | <span data-ttu-id="578a3-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="578a3-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="578a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="578a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="578a3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="578a3-118">Optional query parameters</span></span>
<span data-ttu-id="578a3-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="578a3-119">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="578a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="578a3-120">Request headers</span></span>
| <span data-ttu-id="578a3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="578a3-121">Name</span></span>       | <span data-ttu-id="578a3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="578a3-122">Type</span></span> | <span data-ttu-id="578a3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="578a3-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="578a3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="578a3-124">Authorization</span></span>  | <span data-ttu-id="578a3-125">string</span><span class="sxs-lookup"><span data-stu-id="578a3-125">string</span></span>  | <span data-ttu-id="578a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="578a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="578a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="578a3-128">Request body</span></span>
<span data-ttu-id="578a3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="578a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="578a3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="578a3-130">Response</span></span>

<span data-ttu-id="578a3-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="578a3-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="578a3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="578a3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="578a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="578a3-133">Request</span></span>
<span data-ttu-id="578a3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="578a3-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="578a3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="578a3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="578a3-136">C#</span><span class="sxs-lookup"><span data-stu-id="578a3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="578a3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="578a3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="578a3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="578a3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="578a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="578a3-139">Response</span></span>
<span data-ttu-id="578a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="578a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
