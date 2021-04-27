---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 53d8e550db37d39be37cb566ac1c6b8bbb01200e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046724"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="a78bc-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="a78bc-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="a78bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a78bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a78bc-105">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="a78bc-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a78bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a78bc-106">Permissions</span></span>
<span data-ttu-id="a78bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a78bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a78bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a78bc-109">Permission type</span></span>      | <span data-ttu-id="a78bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a78bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a78bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a78bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a78bc-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a78bc-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a78bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a78bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a78bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a78bc-114">Not supported.</span></span>    |
|<span data-ttu-id="a78bc-115">Application</span><span class="sxs-lookup"><span data-stu-id="a78bc-115">Application</span></span> | <span data-ttu-id="a78bc-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a78bc-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a78bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a78bc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a78bc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a78bc-118">Optional query parameters</span></span>
<span data-ttu-id="a78bc-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="a78bc-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a78bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a78bc-120">Request headers</span></span>
| <span data-ttu-id="a78bc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a78bc-121">Name</span></span>       | <span data-ttu-id="a78bc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a78bc-122">Type</span></span> | <span data-ttu-id="a78bc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a78bc-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a78bc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a78bc-124">Authorization</span></span>  | <span data-ttu-id="a78bc-125">string</span><span class="sxs-lookup"><span data-stu-id="a78bc-125">string</span></span>  | <span data-ttu-id="a78bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a78bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a78bc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a78bc-128">Request body</span></span>
<span data-ttu-id="a78bc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a78bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a78bc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a78bc-130">Response</span></span>

<span data-ttu-id="a78bc-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a78bc-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a78bc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a78bc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a78bc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a78bc-133">Request</span></span>
<span data-ttu-id="a78bc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a78bc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a78bc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a78bc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="a78bc-136">C#</span><span class="sxs-lookup"><span data-stu-id="a78bc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a78bc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a78bc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a78bc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a78bc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a78bc-139">Java</span><span class="sxs-lookup"><span data-stu-id="a78bc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a78bc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a78bc-140">Response</span></span>
<span data-ttu-id="a78bc-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a78bc-141">Here is an example of the response.</span></span> <span data-ttu-id="a78bc-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a78bc-142">Note: The response object shown here might be shortened for readability.</span></span>
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
