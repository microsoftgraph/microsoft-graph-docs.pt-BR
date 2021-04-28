---
title: Listar mailFolders
description: 'Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. '
author: abheek-das
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 3883794642723cc5b7df07ad0c1d1f67fc58aed3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051190"
---
# <a name="list-mailfolders"></a><span data-ttu-id="3782e-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="3782e-103">List mailFolders</span></span>

<span data-ttu-id="3782e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3782e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3782e-105">Obter o conjunto de pastas de email diretamente sob a pasta raiz do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3782e-105">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="3782e-106">O conjunto retornado inclui todas as [pastas de pesquisa de email](../resources/mailsearchfolder.md) diretamente sob a raiz.</span><span class="sxs-lookup"><span data-stu-id="3782e-106">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="3782e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3782e-107">Permissions</span></span>
<span data-ttu-id="3782e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3782e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3782e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3782e-110">Permission type</span></span>      | <span data-ttu-id="3782e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3782e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3782e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3782e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3782e-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3782e-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3782e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3782e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3782e-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3782e-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3782e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3782e-116">Application</span></span> | <span data-ttu-id="3782e-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3782e-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3782e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3782e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3782e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3782e-119">Optional query parameters</span></span>
<span data-ttu-id="3782e-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3782e-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3782e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3782e-121">Request headers</span></span>
| <span data-ttu-id="3782e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3782e-122">Header</span></span>       | <span data-ttu-id="3782e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3782e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3782e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3782e-124">Authorization</span></span>  | <span data-ttu-id="3782e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3782e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3782e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3782e-127">Content-Type</span></span>   | <span data-ttu-id="3782e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3782e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3782e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3782e-129">Request body</span></span>
<span data-ttu-id="3782e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3782e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3782e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3782e-131">Response</span></span>

<span data-ttu-id="3782e-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3782e-132">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3782e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3782e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3782e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3782e-134">Request</span></span>
<span data-ttu-id="3782e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3782e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3782e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3782e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="3782e-137">C#</span><span class="sxs-lookup"><span data-stu-id="3782e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3782e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3782e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3782e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3782e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3782e-140">Java</span><span class="sxs-lookup"><span data-stu-id="3782e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3782e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3782e-141">Response</span></span>
<span data-ttu-id="3782e-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3782e-142">Here is an example of the response.</span></span>

><span data-ttu-id="3782e-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3782e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

