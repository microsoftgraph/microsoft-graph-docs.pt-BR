---
title: Obter contactFolder
description: Obtenha uma pasta de contatos usando a respectiva ID.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 73f9e8359640efa733371b9dd04ba4be6491937a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047095"
---
# <a name="get-contactfolder"></a><span data-ttu-id="a1e50-103">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1e50-103">Get contactFolder</span></span>

<span data-ttu-id="a1e50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1e50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1e50-105">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="a1e50-105">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="a1e50-106">Há dois cenários em que um aplicativo pode obter a pasta de contato de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="a1e50-106">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="a1e50-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="a1e50-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a1e50-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="a1e50-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a1e50-109">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="a1e50-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="a1e50-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1e50-110">Permissions</span></span>
<span data-ttu-id="a1e50-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1e50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e50-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1e50-113">Permission type</span></span>      | <span data-ttu-id="a1e50-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1e50-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1e50-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1e50-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a1e50-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1e50-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a1e50-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1e50-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1e50-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1e50-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a1e50-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1e50-119">Application</span></span> | <span data-ttu-id="a1e50-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1e50-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1e50-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e50-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1e50-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1e50-122">Optional query parameters</span></span>
<span data-ttu-id="a1e50-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e50-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a1e50-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e50-124">Request headers</span></span>
| <span data-ttu-id="a1e50-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a1e50-125">Name</span></span>       | <span data-ttu-id="a1e50-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1e50-126">Type</span></span> | <span data-ttu-id="a1e50-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e50-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1e50-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1e50-128">Authorization</span></span>  | <span data-ttu-id="a1e50-129">string</span><span class="sxs-lookup"><span data-stu-id="a1e50-129">string</span></span>  | <span data-ttu-id="a1e50-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1e50-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1e50-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e50-132">Request body</span></span>
<span data-ttu-id="a1e50-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1e50-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1e50-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e50-134">Response</span></span>

<span data-ttu-id="a1e50-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e50-135">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1e50-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1e50-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1e50-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e50-137">Request</span></span>
<span data-ttu-id="a1e50-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e50-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1e50-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e50-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="a1e50-140">C#</span><span class="sxs-lookup"><span data-stu-id="a1e50-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1e50-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1e50-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1e50-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1e50-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1e50-143">Java</span><span class="sxs-lookup"><span data-stu-id="a1e50-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a1e50-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e50-144">Response</span></span>
<span data-ttu-id="a1e50-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e50-145">Here is an example of the response.</span></span> <span data-ttu-id="a1e50-146">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1e50-146">Note: The response object shown here might be shortened for readability.</span></span>
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
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
