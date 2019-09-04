---
title: Listar directoryRoleTemplates
description: Recupere uma lista de objetos directoryroletemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b0f361216dde9001762c4bb67bbce25c5569a682
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719518"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="1b643-103">Listar directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="1b643-103">List directoryRoleTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b643-104">Recupere uma lista de objetos directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="1b643-104">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b643-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b643-105">Permissions</span></span>
<span data-ttu-id="1b643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b643-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b643-108">Permission type</span></span>      | <span data-ttu-id="1b643-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b643-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b643-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b643-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b643-111">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="1b643-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b643-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b643-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b643-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b643-113">Not supported.</span></span>    |
|<span data-ttu-id="1b643-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b643-114">Application</span></span> | <span data-ttu-id="1b643-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1b643-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b643-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b643-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b643-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b643-117">Optional query parameters</span></span>
<span data-ttu-id="1b643-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="1b643-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b643-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b643-119">Request headers</span></span>
| <span data-ttu-id="1b643-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1b643-120">Name</span></span>       | <span data-ttu-id="1b643-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b643-121">Type</span></span> | <span data-ttu-id="1b643-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b643-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1b643-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b643-123">Authorization</span></span>  | <span data-ttu-id="1b643-124">string</span><span class="sxs-lookup"><span data-stu-id="1b643-124">string</span></span>  | <span data-ttu-id="1b643-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b643-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b643-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b643-127">Request body</span></span>
<span data-ttu-id="1b643-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b643-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b643-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b643-129">Response</span></span>

<span data-ttu-id="1b643-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b643-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b643-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b643-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b643-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b643-132">Request</span></span>
<span data-ttu-id="1b643-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b643-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b643-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b643-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b643-135">C#</span><span class="sxs-lookup"><span data-stu-id="1b643-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b643-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b643-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b643-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1b643-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b643-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b643-138">Response</span></span>
<span data-ttu-id="1b643-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b643-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 139

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
