---
title: Obter contactFolder
description: Obtenha uma pasta de contatos usando a respectiva ID.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cb1f2e9c7a2e3f8870895eba06b7fe3eba8edf85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462158"
---
# <a name="get-contactfolder"></a><span data-ttu-id="4feaf-103">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="4feaf-103">Get contactFolder</span></span>

<span data-ttu-id="4feaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4feaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4feaf-105">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="4feaf-105">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="4feaf-106">Há dois cenários em que um aplicativo pode obter a pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="4feaf-106">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="4feaf-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="4feaf-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="4feaf-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="4feaf-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="4feaf-109">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="4feaf-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="4feaf-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="4feaf-110">Permissions</span></span>
<span data-ttu-id="4feaf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4feaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4feaf-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4feaf-113">Permission type</span></span>      | <span data-ttu-id="4feaf-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4feaf-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4feaf-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4feaf-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4feaf-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4feaf-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4feaf-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4feaf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4feaf-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4feaf-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4feaf-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4feaf-119">Application</span></span> | <span data-ttu-id="4feaf-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4feaf-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4feaf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4feaf-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4feaf-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4feaf-122">Optional query parameters</span></span>
<span data-ttu-id="4feaf-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4feaf-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4feaf-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4feaf-124">Request headers</span></span>
| <span data-ttu-id="4feaf-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4feaf-125">Name</span></span>       | <span data-ttu-id="4feaf-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4feaf-126">Type</span></span> | <span data-ttu-id="4feaf-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4feaf-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4feaf-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="4feaf-128">Authorization</span></span>  | <span data-ttu-id="4feaf-129">string</span><span class="sxs-lookup"><span data-stu-id="4feaf-129">string</span></span>  | <span data-ttu-id="4feaf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4feaf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4feaf-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4feaf-132">Request body</span></span>
<span data-ttu-id="4feaf-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4feaf-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4feaf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4feaf-134">Response</span></span>

<span data-ttu-id="4feaf-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4feaf-135">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4feaf-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4feaf-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4feaf-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4feaf-137">Request</span></span>
<span data-ttu-id="4feaf-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4feaf-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4feaf-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4feaf-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="4feaf-140">C#</span><span class="sxs-lookup"><span data-stu-id="4feaf-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4feaf-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4feaf-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4feaf-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4feaf-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4feaf-143">Java</span><span class="sxs-lookup"><span data-stu-id="4feaf-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4feaf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4feaf-144">Response</span></span>
<span data-ttu-id="4feaf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4feaf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
