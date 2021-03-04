---
title: Listar directoryRoleTemplates
description: Recupere uma lista de objetos directoryroletemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3750e5d036601089d226d64a5e219c1c70fb9cf0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436693"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="6878d-103">Listar directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="6878d-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="6878d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6878d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6878d-105">Recupere uma lista de objetos directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="6878d-105">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6878d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6878d-106">Permissions</span></span>
<span data-ttu-id="6878d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6878d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6878d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6878d-109">Permission type</span></span>      | <span data-ttu-id="6878d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6878d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6878d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6878d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6878d-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6878d-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6878d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6878d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6878d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6878d-114">Not supported.</span></span>    |
|<span data-ttu-id="6878d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6878d-115">Application</span></span> | <span data-ttu-id="6878d-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6878d-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6878d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6878d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6878d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6878d-118">Optional query parameters</span></span>
<span data-ttu-id="6878d-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="6878d-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6878d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6878d-120">Request headers</span></span>
| <span data-ttu-id="6878d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6878d-121">Name</span></span>       | <span data-ttu-id="6878d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6878d-122">Type</span></span> | <span data-ttu-id="6878d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6878d-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6878d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6878d-124">Authorization</span></span>  | <span data-ttu-id="6878d-125">string</span><span class="sxs-lookup"><span data-stu-id="6878d-125">string</span></span>  | <span data-ttu-id="6878d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6878d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6878d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6878d-128">Request body</span></span>
<span data-ttu-id="6878d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6878d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6878d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6878d-130">Response</span></span>

<span data-ttu-id="6878d-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6878d-131">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6878d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6878d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6878d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6878d-133">Request</span></span>
<span data-ttu-id="6878d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6878d-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6878d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6878d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
# <a name="c"></a>[<span data-ttu-id="6878d-136">C#</span><span class="sxs-lookup"><span data-stu-id="6878d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6878d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6878d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6878d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6878d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6878d-139">Java</span><span class="sxs-lookup"><span data-stu-id="6878d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6878d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6878d-140">Response</span></span>
<span data-ttu-id="6878d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6878d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
