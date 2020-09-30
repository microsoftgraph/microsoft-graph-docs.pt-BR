---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 378795707b0cdcff9b2bb1c45d257078b68189e3
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312854"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="2aeda-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="2aeda-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="2aeda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2aeda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aeda-105">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="2aeda-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2aeda-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2aeda-106">Permissions</span></span>
<span data-ttu-id="2aeda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aeda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aeda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2aeda-109">Permission type</span></span>      | <span data-ttu-id="2aeda-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2aeda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2aeda-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2aeda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2aeda-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="2aeda-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2aeda-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2aeda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2aeda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2aeda-114">Not supported.</span></span>    |
|<span data-ttu-id="2aeda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2aeda-115">Application</span></span> | <span data-ttu-id="2aeda-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2aeda-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2aeda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2aeda-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2aeda-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2aeda-118">Optional query parameters</span></span>
<span data-ttu-id="2aeda-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="2aeda-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2aeda-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2aeda-120">Request headers</span></span>
| <span data-ttu-id="2aeda-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2aeda-121">Name</span></span>       | <span data-ttu-id="2aeda-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2aeda-122">Type</span></span> | <span data-ttu-id="2aeda-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aeda-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2aeda-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2aeda-124">Authorization</span></span>  | <span data-ttu-id="2aeda-125">string</span><span class="sxs-lookup"><span data-stu-id="2aeda-125">string</span></span>  | <span data-ttu-id="2aeda-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2aeda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2aeda-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2aeda-128">Request body</span></span>
<span data-ttu-id="2aeda-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2aeda-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2aeda-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2aeda-130">Response</span></span>

<span data-ttu-id="2aeda-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2aeda-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2aeda-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2aeda-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2aeda-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2aeda-133">Request</span></span>
<span data-ttu-id="2aeda-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2aeda-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2aeda-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2aeda-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="2aeda-136">C#</span><span class="sxs-lookup"><span data-stu-id="2aeda-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2aeda-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aeda-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2aeda-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2aeda-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2aeda-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2aeda-139">Response</span></span>
<span data-ttu-id="2aeda-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2aeda-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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