---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad72fd78b377d144e66664667465560e9893372e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457804"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="ca2a2-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="ca2a2-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="ca2a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca2a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca2a2-105">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca2a2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ca2a2-106">Permissions</span></span>
<span data-ttu-id="ca2a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca2a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca2a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca2a2-109">Permission type</span></span>      | <span data-ttu-id="ca2a2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca2a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca2a2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca2a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca2a2-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ca2a2-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca2a2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca2a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca2a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-114">Not supported.</span></span>    |
|<span data-ttu-id="ca2a2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca2a2-115">Application</span></span> | <span data-ttu-id="ca2a2-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ca2a2-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca2a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca2a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca2a2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca2a2-118">Optional query parameters</span></span>
<span data-ttu-id="ca2a2-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="ca2a2-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca2a2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2a2-120">Request headers</span></span>
| <span data-ttu-id="ca2a2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ca2a2-121">Name</span></span>       | <span data-ttu-id="ca2a2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca2a2-122">Type</span></span> | <span data-ttu-id="ca2a2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca2a2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca2a2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca2a2-124">Authorization</span></span>  | <span data-ttu-id="ca2a2-125">string</span><span class="sxs-lookup"><span data-stu-id="ca2a2-125">string</span></span>  | <span data-ttu-id="ca2a2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca2a2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2a2-128">Request body</span></span>
<span data-ttu-id="ca2a2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca2a2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca2a2-130">Response</span></span>

<span data-ttu-id="ca2a2-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca2a2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca2a2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca2a2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2a2-133">Request</span></span>
<span data-ttu-id="ca2a2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca2a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca2a2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="ca2a2-136">C#</span><span class="sxs-lookup"><span data-stu-id="ca2a2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca2a2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca2a2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca2a2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca2a2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca2a2-139">Java</span><span class="sxs-lookup"><span data-stu-id="ca2a2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca2a2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca2a2-140">Response</span></span>
<span data-ttu-id="ca2a2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
