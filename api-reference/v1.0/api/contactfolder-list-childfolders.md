---
title: Listar childFolders
description: Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8dc0e3297f6bc1142fdf5dc8e66c9d38315705bf
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459211"
---
# <a name="list-childfolders"></a><span data-ttu-id="6870f-103">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="6870f-103">List childFolders</span></span>

<span data-ttu-id="6870f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6870f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6870f-105">Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="6870f-105">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="6870f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6870f-106">Permissions</span></span>
<span data-ttu-id="6870f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6870f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6870f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6870f-109">Permission type</span></span>      | <span data-ttu-id="6870f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6870f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6870f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6870f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6870f-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6870f-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6870f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6870f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6870f-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6870f-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6870f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6870f-115">Application</span></span> | <span data-ttu-id="6870f-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6870f-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6870f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6870f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6870f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6870f-118">Optional query parameters</span></span>
<span data-ttu-id="6870f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6870f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6870f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6870f-120">Request headers</span></span>
| <span data-ttu-id="6870f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6870f-121">Name</span></span>       | <span data-ttu-id="6870f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6870f-122">Type</span></span> | <span data-ttu-id="6870f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6870f-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6870f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6870f-124">Authorization</span></span>  | <span data-ttu-id="6870f-125">string</span><span class="sxs-lookup"><span data-stu-id="6870f-125">string</span></span>  | <span data-ttu-id="6870f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6870f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6870f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6870f-128">Request body</span></span>
<span data-ttu-id="6870f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6870f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6870f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6870f-130">Response</span></span>

<span data-ttu-id="6870f-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6870f-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6870f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6870f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6870f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6870f-133">Request</span></span>
<span data-ttu-id="6870f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6870f-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6870f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6870f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="6870f-136">C#</span><span class="sxs-lookup"><span data-stu-id="6870f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6870f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6870f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6870f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6870f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6870f-139">Java</span><span class="sxs-lookup"><span data-stu-id="6870f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6870f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6870f-140">Response</span></span>
<span data-ttu-id="6870f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6870f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
