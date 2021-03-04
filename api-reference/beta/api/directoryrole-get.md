---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 70d72048536c3e2516beb296c6f2412a64e5b96f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436789"
---
# <a name="get-directoryrole"></a><span data-ttu-id="06024-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="06024-103">Get directoryRole</span></span>

<span data-ttu-id="06024-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06024-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06024-105">Recupere as propriedades de um objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="06024-105">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06024-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="06024-106">Permissions</span></span>
<span data-ttu-id="06024-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06024-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06024-109">Permission type</span></span>      | <span data-ttu-id="06024-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06024-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06024-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06024-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06024-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06024-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06024-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06024-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06024-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06024-114">Not supported.</span></span>    |
|<span data-ttu-id="06024-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06024-115">Application</span></span> | <span data-ttu-id="06024-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06024-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06024-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06024-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06024-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06024-118">Optional query parameters</span></span>
<span data-ttu-id="06024-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="06024-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06024-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06024-120">Request headers</span></span>
| <span data-ttu-id="06024-121">Nome</span><span class="sxs-lookup"><span data-stu-id="06024-121">Name</span></span>       | <span data-ttu-id="06024-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="06024-122">Type</span></span> | <span data-ttu-id="06024-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="06024-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06024-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="06024-124">Authorization</span></span>  | <span data-ttu-id="06024-125">string</span><span class="sxs-lookup"><span data-stu-id="06024-125">string</span></span>  | <span data-ttu-id="06024-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06024-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06024-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06024-128">Request body</span></span>
<span data-ttu-id="06024-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06024-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06024-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="06024-130">Response</span></span>

<span data-ttu-id="06024-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06024-131">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06024-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06024-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06024-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06024-133">Request</span></span>
<span data-ttu-id="06024-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06024-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06024-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="06024-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="06024-136">C#</span><span class="sxs-lookup"><span data-stu-id="06024-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06024-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06024-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06024-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06024-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06024-139">Java</span><span class="sxs-lookup"><span data-stu-id="06024-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06024-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="06024-140">Response</span></span>
<span data-ttu-id="06024-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06024-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
