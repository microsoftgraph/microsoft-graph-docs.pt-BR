---
title: Listar mailFolders
description: Obtenha todas as pastas de email na caixa de correio do usuário conectado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: af3a6970edf051da3cce2c5fc51458ea6f45a388
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812846"
---
# <a name="list-mailfolders"></a><span data-ttu-id="37328-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="37328-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37328-104">Obtenha todas as pastas de email na caixa de correio do usuário conectado, incluindo as [pastas de pesquisa de email](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="37328-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37328-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="37328-105">Permissions</span></span>
<span data-ttu-id="37328-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37328-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37328-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37328-108">Permission type</span></span>      | <span data-ttu-id="37328-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37328-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37328-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37328-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37328-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37328-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="37328-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37328-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37328-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37328-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="37328-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37328-114">Application</span></span> | <span data-ttu-id="37328-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37328-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="37328-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37328-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37328-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37328-117">Optional query parameters</span></span>
<span data-ttu-id="37328-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37328-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="37328-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37328-119">Request headers</span></span>
| <span data-ttu-id="37328-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37328-120">Header</span></span>       | <span data-ttu-id="37328-121">Valor</span><span class="sxs-lookup"><span data-stu-id="37328-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37328-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37328-122">Authorization</span></span>  | <span data-ttu-id="37328-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37328-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37328-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37328-125">Content-Type</span></span>   | <span data-ttu-id="37328-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37328-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37328-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37328-127">Request body</span></span>
<span data-ttu-id="37328-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37328-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37328-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="37328-129">Response</span></span>

<span data-ttu-id="37328-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37328-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37328-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37328-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37328-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37328-132">Request</span></span>
<span data-ttu-id="37328-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37328-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="37328-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="37328-134">Response</span></span>
<span data-ttu-id="37328-135">Veja um exemplo da resposta que inclui um **mailSearchFolder** que é uma pasta filha na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="37328-135">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="37328-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="37328-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="37328-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37328-137">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="37328-138">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="37328-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="37328-139">C#</span><span class="sxs-lookup"><span data-stu-id="37328-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37328-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="37328-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
