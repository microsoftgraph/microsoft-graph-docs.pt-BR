---
title: Obter mailFolder
description: Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1bd8a4f49d329cb4123f0ffcde142b2591c60132
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728738"
---
# <a name="get-mailfolder"></a><span data-ttu-id="db75c-103">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="db75c-103">Get mailFolder</span></span>

<span data-ttu-id="db75c-104">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="db75c-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="db75c-105">Existem dois cenários em que um aplicativo pode receber a pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="db75c-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="db75c-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="db75c-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="db75c-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="db75c-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="db75c-108">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="db75c-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="db75c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="db75c-109">Permissions</span></span>
<span data-ttu-id="db75c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db75c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db75c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db75c-112">Permission type</span></span>      | <span data-ttu-id="db75c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db75c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db75c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db75c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="db75c-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db75c-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db75c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db75c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db75c-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db75c-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db75c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db75c-118">Application</span></span> | <span data-ttu-id="db75c-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db75c-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db75c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db75c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db75c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db75c-121">Optional query parameters</span></span>
<span data-ttu-id="db75c-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="db75c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="db75c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db75c-123">Request headers</span></span>
| <span data-ttu-id="db75c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="db75c-124">Name</span></span>       | <span data-ttu-id="db75c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="db75c-125">Type</span></span> | <span data-ttu-id="db75c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="db75c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db75c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="db75c-127">Authorization</span></span>  | <span data-ttu-id="db75c-128">string</span><span class="sxs-lookup"><span data-stu-id="db75c-128">string</span></span>  | <span data-ttu-id="db75c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db75c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db75c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db75c-131">Request body</span></span>
<span data-ttu-id="db75c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db75c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db75c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="db75c-133">Response</span></span>

<span data-ttu-id="db75c-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db75c-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="db75c-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db75c-135">Examples</span></span>
### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="db75c-136">Exemplo 1: obter uma pasta de email</span><span class="sxs-lookup"><span data-stu-id="db75c-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="db75c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db75c-137">Request</span></span>

<span data-ttu-id="db75c-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db75c-138">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db75c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="db75c-139">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db75c-140">C#</span><span class="sxs-lookup"><span data-stu-id="db75c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db75c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db75c-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db75c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db75c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db75c-143">Java</span><span class="sxs-lookup"><span data-stu-id="db75c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db75c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="db75c-144">Response</span></span>

<span data-ttu-id="db75c-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db75c-145">The following is an example of the response.</span></span>

> <span data-ttu-id="db75c-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db75c-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db75c-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db75c-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGVmMDEzM",
  "displayName": "Inbox",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 2,
  "unreadItemCount": 59,
  "totalItemCount": 60,
  "wellKnownName": "inbox"
}
```

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="db75c-148">Exemplo 2: obter uma pasta de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="db75c-148">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="db75c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db75c-149">Request</span></span>

<span data-ttu-id="db75c-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db75c-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db75c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="db75c-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db75c-152">C#</span><span class="sxs-lookup"><span data-stu-id="db75c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db75c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db75c-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db75c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db75c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db75c-155">Java</span><span class="sxs-lookup"><span data-stu-id="db75c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db75c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="db75c-156">Response</span></span>

<span data-ttu-id="db75c-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db75c-157">The following is an example of the response.</span></span>

> <span data-ttu-id="db75c-158">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db75c-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db75c-159">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db75c-159">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
