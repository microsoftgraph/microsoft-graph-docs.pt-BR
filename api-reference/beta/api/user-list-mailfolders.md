---
title: Listar mailFolders
description: Obtenha todas as pastas de email na caixa de correio do usuário conectado.
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ecffc08e39b21afff4818d25a98a6fc1d2156c43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987618"
---
# <a name="list-mailfolders"></a><span data-ttu-id="085f9-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="085f9-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="085f9-104">Obtenha todas as pastas de email na caixa de correio do usuário conectado, incluindo as [pastas de pesquisa de email](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="085f9-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="085f9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="085f9-105">Permissions</span></span>
<span data-ttu-id="085f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="085f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="085f9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="085f9-108">Permission type</span></span>      | <span data-ttu-id="085f9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="085f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="085f9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="085f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="085f9-111">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="085f9-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="085f9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="085f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="085f9-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="085f9-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="085f9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="085f9-114">Application</span></span> | <span data-ttu-id="085f9-115">Mail. ReadBasic. All, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="085f9-115">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="085f9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="085f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="085f9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="085f9-117">Optional query parameters</span></span>
<span data-ttu-id="085f9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="085f9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="085f9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="085f9-119">Request headers</span></span>
| <span data-ttu-id="085f9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="085f9-120">Header</span></span>       | <span data-ttu-id="085f9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="085f9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="085f9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="085f9-122">Authorization</span></span>  | <span data-ttu-id="085f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="085f9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="085f9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="085f9-125">Content-Type</span></span>   | <span data-ttu-id="085f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="085f9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="085f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="085f9-127">Request body</span></span>
<span data-ttu-id="085f9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="085f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="085f9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="085f9-129">Response</span></span>

<span data-ttu-id="085f9-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="085f9-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="085f9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="085f9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="085f9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="085f9-132">Request</span></span>
<span data-ttu-id="085f9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="085f9-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="085f9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="085f9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="085f9-135">C#</span><span class="sxs-lookup"><span data-stu-id="085f9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="085f9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="085f9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="085f9-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="085f9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="085f9-138">Java</span><span class="sxs-lookup"><span data-stu-id="085f9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="085f9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="085f9-139">Response</span></span>
<span data-ttu-id="085f9-140">Veja um exemplo da resposta que inclui um **mailSearchFolder** que é uma pasta filha na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="085f9-140">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="085f9-141">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="085f9-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="085f9-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="085f9-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "archive"
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory"
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems"
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts"
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox"
        },
        {
            "@odata.type": "#microsoft.graph.mailSearchFolder",
            "id": "AAMkADYRAAAZg1yTAAA=",
            "displayName": "Weekly digests",
            "parentFolderId": "AQMkADYAAAIBDAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 4,
            "totalItemCount": 5,
            "wellKnownName": null,
            "isSupported": true,
            "filterQuery": "contains(subject, 'weekly digest')"
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "junkemail"
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox"
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
