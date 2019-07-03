---
title: Listar childFolders
description: Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c046bd3a9396e3d96df4ca989444b6e4888c15ee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443003"
---
# <a name="list-childfolders"></a><span data-ttu-id="21f08-103">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="21f08-103">List childFolders</span></span>

<span data-ttu-id="21f08-104">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="21f08-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="21f08-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="21f08-105">Permissions</span></span>
<span data-ttu-id="21f08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21f08-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21f08-108">Permission type</span></span>      | <span data-ttu-id="21f08-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21f08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21f08-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21f08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21f08-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21f08-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="21f08-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21f08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21f08-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21f08-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="21f08-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21f08-114">Application</span></span> | <span data-ttu-id="21f08-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21f08-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="21f08-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21f08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="21f08-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21f08-117">Optional query parameters</span></span>
<span data-ttu-id="21f08-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21f08-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="21f08-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21f08-119">Request headers</span></span>
| <span data-ttu-id="21f08-120">Nome</span><span class="sxs-lookup"><span data-stu-id="21f08-120">Name</span></span>       | <span data-ttu-id="21f08-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="21f08-121">Type</span></span> | <span data-ttu-id="21f08-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="21f08-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="21f08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21f08-123">Authorization</span></span>  | <span data-ttu-id="21f08-124">string</span><span class="sxs-lookup"><span data-stu-id="21f08-124">string</span></span>  | <span data-ttu-id="21f08-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21f08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21f08-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21f08-127">Request body</span></span>
<span data-ttu-id="21f08-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21f08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21f08-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="21f08-129">Response</span></span>

<span data-ttu-id="21f08-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21f08-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21f08-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21f08-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21f08-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21f08-132">Request</span></span>
<span data-ttu-id="21f08-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21f08-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21f08-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="21f08-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21f08-135">C#</span><span class="sxs-lookup"><span data-stu-id="21f08-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21f08-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="21f08-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21f08-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="21f08-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="21f08-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="21f08-138">Response</span></span>
<span data-ttu-id="21f08-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21f08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
