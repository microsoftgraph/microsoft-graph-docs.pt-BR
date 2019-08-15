---
title: Listar mailFolders
description: Obtenha todas as pastas de email na caixa de correio do usuário conectado.
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6c218346a50666af625013b4b8ca1959c046d991
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408963"
---
# <a name="list-mailfolders"></a><span data-ttu-id="3436a-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="3436a-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3436a-104">Obtenha todas as pastas de email na caixa de correio do usuário conectado, incluindo as [pastas de pesquisa de email](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3436a-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3436a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3436a-105">Permissions</span></span>
<span data-ttu-id="3436a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3436a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3436a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3436a-108">Permission type</span></span>      | <span data-ttu-id="3436a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3436a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3436a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3436a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3436a-111">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3436a-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3436a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3436a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3436a-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3436a-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3436a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3436a-114">Application</span></span> | <span data-ttu-id="3436a-115">Mail. ReadBasic. All, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3436a-115">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3436a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3436a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3436a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3436a-117">Optional query parameters</span></span>
<span data-ttu-id="3436a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3436a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3436a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3436a-119">Request headers</span></span>
| <span data-ttu-id="3436a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3436a-120">Header</span></span>       | <span data-ttu-id="3436a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3436a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3436a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3436a-122">Authorization</span></span>  | <span data-ttu-id="3436a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3436a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3436a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3436a-125">Content-Type</span></span>   | <span data-ttu-id="3436a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3436a-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3436a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3436a-127">Request body</span></span>
<span data-ttu-id="3436a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3436a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3436a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3436a-129">Response</span></span>

<span data-ttu-id="3436a-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3436a-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3436a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3436a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3436a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3436a-132">Request</span></span>
<span data-ttu-id="3436a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3436a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3436a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3436a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3436a-135">C#</span><span class="sxs-lookup"><span data-stu-id="3436a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3436a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3436a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3436a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3436a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3436a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3436a-138">Response</span></span>
<span data-ttu-id="3436a-139">Veja um exemplo da resposta que inclui um **mailSearchFolder** que é uma pasta filha na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="3436a-139">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="3436a-140">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3436a-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3436a-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3436a-141">All of the properties will be returned from an actual call.</span></span>
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
