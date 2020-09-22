---
title: Listar mailFolders
description: Obtenha todas as pastas de email na caixa de correio do usuário conectado.
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: outlook
ms.openlocfilehash: 757fb07765bcbe693909d422c5d4bdad2bd0c9e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016889"
---
# <a name="list-mailfolders"></a><span data-ttu-id="6b325-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="6b325-103">List mailFolders</span></span>

<span data-ttu-id="6b325-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b325-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b325-105">Obtenha todas as pastas de email na caixa de correio do usuário conectado, incluindo as [pastas de pesquisa de email](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6b325-105">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b325-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b325-106">Permissions</span></span>
<span data-ttu-id="6b325-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b325-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b325-109">Permission type</span></span>      | <span data-ttu-id="6b325-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b325-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b325-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b325-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b325-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b325-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6b325-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b325-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b325-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b325-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6b325-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b325-115">Application</span></span> | <span data-ttu-id="6b325-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b325-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b325-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b325-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b325-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b325-118">Optional query parameters</span></span>
<span data-ttu-id="6b325-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b325-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6b325-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b325-120">Request headers</span></span>
| <span data-ttu-id="6b325-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b325-121">Header</span></span>       | <span data-ttu-id="6b325-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b325-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b325-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b325-123">Authorization</span></span>  | <span data-ttu-id="6b325-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b325-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b325-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b325-126">Content-Type</span></span>   | <span data-ttu-id="6b325-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6b325-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b325-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b325-128">Request body</span></span>
<span data-ttu-id="6b325-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b325-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b325-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b325-130">Response</span></span>

<span data-ttu-id="6b325-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b325-131">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b325-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b325-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b325-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b325-133">Request</span></span>
<span data-ttu-id="6b325-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b325-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b325-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b325-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="6b325-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b325-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b325-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b325-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b325-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b325-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b325-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b325-139">Response</span></span>
<span data-ttu-id="6b325-140">Veja um exemplo da resposta que inclui um **mailSearchFolder** que é uma pasta filha na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="6b325-140">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="6b325-141">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6b325-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6b325-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b325-142">All of the properties will be returned from an actual call.</span></span>
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


