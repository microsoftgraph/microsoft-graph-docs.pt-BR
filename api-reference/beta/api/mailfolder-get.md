---
title: Obter mailFolder
description: Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 55cdf16f564f4e780871ec77530384b4ff4c2c7f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401824"
---
# <a name="get-mailfolder"></a><span data-ttu-id="8939a-103">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="8939a-103">Get mailFolder</span></span>

<span data-ttu-id="8939a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8939a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8939a-105">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="8939a-105">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="8939a-106">Existem dois cenários em que um aplicativo pode receber a pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="8939a-106">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="8939a-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="8939a-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8939a-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="8939a-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8939a-109">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="8939a-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="8939a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8939a-110">Permissions</span></span>

<span data-ttu-id="8939a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8939a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8939a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8939a-113">Permission type</span></span>      | <span data-ttu-id="8939a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8939a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8939a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8939a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8939a-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8939a-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8939a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8939a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8939a-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8939a-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8939a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8939a-119">Application</span></span> | <span data-ttu-id="8939a-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8939a-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8939a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8939a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8939a-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8939a-122">Optional query parameters</span></span>

<span data-ttu-id="8939a-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8939a-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8939a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8939a-124">Request headers</span></span>

| <span data-ttu-id="8939a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8939a-125">Name</span></span>          | <span data-ttu-id="8939a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8939a-126">Type</span></span>   | <span data-ttu-id="8939a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8939a-127">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="8939a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8939a-128">Authorization</span></span> | <span data-ttu-id="8939a-129">string</span><span class="sxs-lookup"><span data-stu-id="8939a-129">string</span></span> | <span data-ttu-id="8939a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8939a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8939a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8939a-132">Request body</span></span>

<span data-ttu-id="8939a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8939a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8939a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8939a-134">Response</span></span>

<span data-ttu-id="8939a-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8939a-135">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8939a-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8939a-136">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="8939a-137">Exemplo 1: obter uma pasta de email</span><span class="sxs-lookup"><span data-stu-id="8939a-137">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="8939a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8939a-138">Request</span></span>

<span data-ttu-id="8939a-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8939a-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8939a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8939a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="c"></a>[<span data-ttu-id="8939a-141">C#</span><span class="sxs-lookup"><span data-stu-id="8939a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8939a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8939a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8939a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8939a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8939a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8939a-144">Response</span></span>

<span data-ttu-id="8939a-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8939a-145">The following is an example of the response.</span></span>

> <span data-ttu-id="8939a-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8939a-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8939a-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8939a-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="8939a-148">Exemplo 2: obter uma pasta de pesquisa de email</span><span class="sxs-lookup"><span data-stu-id="8939a-148">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="8939a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8939a-149">Request</span></span>

<span data-ttu-id="8939a-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8939a-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8939a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8939a-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="c"></a>[<span data-ttu-id="8939a-152">C#</span><span class="sxs-lookup"><span data-stu-id="8939a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8939a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8939a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8939a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8939a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8939a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8939a-155">Response</span></span>

<span data-ttu-id="8939a-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8939a-156">The following is an example of the response.</span></span>

> <span data-ttu-id="8939a-157">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8939a-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8939a-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8939a-158">All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->