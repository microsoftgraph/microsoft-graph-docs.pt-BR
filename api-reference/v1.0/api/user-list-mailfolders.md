---
title: Listar mailFolders
description: 'Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 30ade50ea548e9310ca5971c8ba4b7b1212d096d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893834"
---
# <a name="list-mailfolders"></a><span data-ttu-id="9fb98-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="9fb98-103">List mailFolders</span></span>

<span data-ttu-id="9fb98-104">Obter o conjunto de pastas de email diretamente sob a pasta raiz do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9fb98-104">Get the mail folder collection under the root folder of the signed-in user.</span></span> <span data-ttu-id="9fb98-105">O conjunto retornado inclui todas as [pastas de pesquisa de email](../resources/mailsearchfolder.md) diretamente sob a raiz.</span><span class="sxs-lookup"><span data-stu-id="9fb98-105">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fb98-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fb98-106">Permissions</span></span>
<span data-ttu-id="9fb98-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb98-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fb98-109">Permission type</span></span>      | <span data-ttu-id="9fb98-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fb98-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fb98-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fb98-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9fb98-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fb98-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9fb98-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fb98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb98-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fb98-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9fb98-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fb98-115">Application</span></span> | <span data-ttu-id="9fb98-116">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fb98-116">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb98-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb98-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9fb98-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9fb98-118">Optional query parameters</span></span>
<span data-ttu-id="9fb98-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9fb98-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9fb98-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb98-120">Request headers</span></span>
| <span data-ttu-id="9fb98-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fb98-121">Header</span></span>       | <span data-ttu-id="9fb98-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9fb98-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9fb98-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fb98-123">Authorization</span></span>  | <span data-ttu-id="9fb98-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb98-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9fb98-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9fb98-126">Content-Type</span></span>   | <span data-ttu-id="9fb98-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9fb98-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9fb98-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb98-128">Request body</span></span>
<span data-ttu-id="9fb98-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fb98-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fb98-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fb98-130">Response</span></span>

<span data-ttu-id="9fb98-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fb98-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9fb98-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fb98-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fb98-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb98-133">Request</span></span>
<span data-ttu-id="9fb98-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fb98-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fb98-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb98-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fb98-136">C#</span><span class="sxs-lookup"><span data-stu-id="9fb98-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fb98-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9fb98-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fb98-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fb98-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fb98-139">Java</span><span class="sxs-lookup"><span data-stu-id="9fb98-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9fb98-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fb98-140">Response</span></span>
<span data-ttu-id="9fb98-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fb98-141">Here is an example of the response.</span></span> 

><span data-ttu-id="9fb98-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fb98-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

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
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
