---
title: Listar directoryRoleTemplates
description: Recupere uma lista de objetos directoryRoleTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a15ac02372e6738daaae70d2ff07965b616c67fc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375335"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="db43f-103">Listar directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="db43f-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="db43f-104">Recupere uma lista de objetos directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="db43f-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="db43f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db43f-105">Permissions</span></span>
<span data-ttu-id="db43f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db43f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db43f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db43f-108">Permission type</span></span>      | <span data-ttu-id="db43f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db43f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db43f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db43f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db43f-111">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="db43f-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db43f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db43f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db43f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db43f-113">Not supported.</span></span>    |
|<span data-ttu-id="db43f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db43f-114">Application</span></span> | <span data-ttu-id="db43f-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="db43f-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db43f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db43f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db43f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db43f-117">Optional query parameters</span></span>
<span data-ttu-id="db43f-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="db43f-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db43f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db43f-119">Request headers</span></span>
| <span data-ttu-id="db43f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="db43f-120">Name</span></span>       | <span data-ttu-id="db43f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="db43f-121">Type</span></span> | <span data-ttu-id="db43f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="db43f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db43f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db43f-123">Authorization</span></span>  | <span data-ttu-id="db43f-124">string</span><span class="sxs-lookup"><span data-stu-id="db43f-124">string</span></span>  | <span data-ttu-id="db43f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db43f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db43f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db43f-127">Request body</span></span>
<span data-ttu-id="db43f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db43f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db43f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="db43f-129">Response</span></span>

<span data-ttu-id="db43f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db43f-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db43f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db43f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db43f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db43f-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db43f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db43f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db43f-134">C#</span><span class="sxs-lookup"><span data-stu-id="db43f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db43f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db43f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db43f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db43f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db43f-137">Java</span><span class="sxs-lookup"><span data-stu-id="db43f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db43f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="db43f-138">Response</span></span>
<span data-ttu-id="db43f-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db43f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
