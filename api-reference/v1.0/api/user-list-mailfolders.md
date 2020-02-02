---
title: Listar mailFolders
description: 'Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. '
author: angelgolfer-ms
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 1b802b636ce4a2a7e3b0b4b3c9c3c145842a9670
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652225"
---
# <a name="list-mailfolders"></a><span data-ttu-id="53766-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="53766-103">List mailFolders</span></span>

<span data-ttu-id="53766-104">Obter o conjunto de pastas de email diretamente sob a pasta raiz do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="53766-104">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="53766-105">O conjunto retornado inclui todas as [pastas de pesquisa de email](../resources/mailsearchfolder.md) diretamente sob a raiz.</span><span class="sxs-lookup"><span data-stu-id="53766-105">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="53766-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="53766-106">Permissions</span></span>
<span data-ttu-id="53766-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53766-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53766-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53766-109">Permission type</span></span>      | <span data-ttu-id="53766-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53766-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53766-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53766-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53766-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53766-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53766-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53766-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53766-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53766-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53766-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53766-115">Application</span></span> | <span data-ttu-id="53766-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53766-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="53766-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53766-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53766-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="53766-118">Optional query parameters</span></span>
<span data-ttu-id="53766-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="53766-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53766-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53766-120">Request headers</span></span>
| <span data-ttu-id="53766-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53766-121">Header</span></span>       | <span data-ttu-id="53766-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53766-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53766-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53766-123">Authorization</span></span>  | <span data-ttu-id="53766-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53766-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="53766-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53766-126">Content-Type</span></span>   | <span data-ttu-id="53766-127">application/json</span><span class="sxs-lookup"><span data-stu-id="53766-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53766-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53766-128">Request body</span></span>
<span data-ttu-id="53766-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53766-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53766-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="53766-130">Response</span></span>

<span data-ttu-id="53766-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53766-131">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53766-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53766-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53766-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53766-133">Request</span></span>
<span data-ttu-id="53766-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53766-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53766-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="53766-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53766-136">C#</span><span class="sxs-lookup"><span data-stu-id="53766-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53766-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53766-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53766-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53766-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53766-139">Java</span><span class="sxs-lookup"><span data-stu-id="53766-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53766-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="53766-140">Response</span></span>
<span data-ttu-id="53766-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53766-141">Here is an example of the response.</span></span>

><span data-ttu-id="53766-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53766-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
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
