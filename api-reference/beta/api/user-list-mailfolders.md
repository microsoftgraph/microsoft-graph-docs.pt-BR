---
title: Listar mailFolders
description: Obtenha todas as pastas de email na caixa de correio do usuário conectado.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: c2cf43dc9d01ba2de2a3426cce84aaf3f92bbbb3
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768190"
---
# <a name="list-mailfolders"></a><span data-ttu-id="1eb48-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="1eb48-103">List mailFolders</span></span>

<span data-ttu-id="1eb48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eb48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb48-105">Obtenha todas as pastas de email na caixa de correio do usuário especificado, incluindo as [pastas de pesquisa de email](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1eb48-105">Get all the mail folders in the specified user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="1eb48-106">Por padrão, essa operação não retorna pastas ocultas.</span><span class="sxs-lookup"><span data-stu-id="1eb48-106">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="1eb48-107">Use um parâmetro de consulta _includeHiddenFolders_ para incluí-los na resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb48-107">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="1eb48-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="1eb48-108">Permissions</span></span>
<span data-ttu-id="1eb48-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eb48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb48-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eb48-111">Permission type</span></span>      | <span data-ttu-id="1eb48-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1eb48-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1eb48-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eb48-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1eb48-114">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1eb48-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1eb48-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eb48-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1eb48-116">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1eb48-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1eb48-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1eb48-117">Application</span></span> | <span data-ttu-id="1eb48-118">Mail. ReadBasic. All, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1eb48-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1eb48-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb48-119">HTTP request</span></span>

<span data-ttu-id="1eb48-120">Para obter todas as pastas de email na caixa de correio do usuário especificado, excluindo as que estão ocultas:</span><span class="sxs-lookup"><span data-stu-id="1eb48-120">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="1eb48-121">Para incluir pastas de email _ocultas_ na resposta:</span><span class="sxs-lookup"><span data-stu-id="1eb48-121">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="query-parameters"></a><span data-ttu-id="1eb48-122">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="1eb48-122">Query parameters</span></span>
<span data-ttu-id="1eb48-123">Para retornar uma lista de todos os mailFolders incluindo aqueles que estão ocultos (sua propriedade **IsHidden** é true), na URL de solicitação, especifique o `includeHiddenFolders` parâmetro de consulta como `true` , conforme mostrado na seção [solicitação HTTP](#http-request) .</span><span class="sxs-lookup"><span data-stu-id="1eb48-123">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="1eb48-124">Este método também dá suporte a [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb48-124">This method also supports [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1eb48-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb48-125">Request headers</span></span>
| <span data-ttu-id="1eb48-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1eb48-126">Header</span></span>       | <span data-ttu-id="1eb48-127">Valor</span><span class="sxs-lookup"><span data-stu-id="1eb48-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1eb48-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eb48-128">Authorization</span></span>  | <span data-ttu-id="1eb48-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1eb48-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1eb48-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb48-131">Request body</span></span>
<span data-ttu-id="1eb48-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1eb48-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eb48-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb48-133">Response</span></span>

<span data-ttu-id="1eb48-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailfolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb48-134">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="1eb48-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1eb48-135">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="1eb48-136">Exemplo 1: listar pastas de email na caixa de correio do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="1eb48-136">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="1eb48-137">Este exemplo inclui um objeto **mailSearchFolder** na resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb48-137">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="1eb48-138">A pasta de pesquisa de email é uma pasta filha na caixa de entrada com o nome de exibição "resumos semanais".</span><span class="sxs-lookup"><span data-stu-id="1eb48-138">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="1eb48-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb48-139">Request</span></span>
<span data-ttu-id="1eb48-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eb48-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1eb48-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb48-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="1eb48-142">C#</span><span class="sxs-lookup"><span data-stu-id="1eb48-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1eb48-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1eb48-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1eb48-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1eb48-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1eb48-145">Java</span><span class="sxs-lookup"><span data-stu-id="1eb48-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1eb48-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb48-146">Response</span></span>
<span data-ttu-id="1eb48-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb48-147">Here is an example of the response.</span></span> 

><span data-ttu-id="1eb48-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1eb48-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
            "wellKnownName": "archive",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox",
            "isHidden": false
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
            "isHidden": false,
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
            "wellKnownName": "junkemail",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems",
            "isHidden": false
        }
    ]
}
```


### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="1eb48-149">Exemplo 2: incluir pastas ocultas na caixa de correio do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="1eb48-149">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="1eb48-150">O exemplo a seguir usa o `includeHiddenFolders` parâmetro de consulta para obter uma lista de pastas de email, incluindo pastas de email ocultas.</span><span class="sxs-lookup"><span data-stu-id="1eb48-150">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="1eb48-151">A resposta inclui a pasta "resíduos" que tem o **IsHidden** definido como true.</span><span class="sxs-lookup"><span data-stu-id="1eb48-151">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="1eb48-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb48-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1eb48-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb48-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="1eb48-154">C#</span><span class="sxs-lookup"><span data-stu-id="1eb48-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hiddenmailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1eb48-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1eb48-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hiddenmailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1eb48-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1eb48-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hiddenmailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1eb48-157">Java</span><span class="sxs-lookup"><span data-stu-id="1eb48-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hiddenmailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1eb48-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb48-158">Response</span></span>
<span data-ttu-id="1eb48-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb48-159">Here is an example of the response.</span></span>

><span data-ttu-id="1eb48-160">**Observação:** O objeto de resposta mostrado aqui é reduzido para legibilidade e não inclui todas as pastas padrão em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="1eb48-160">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Clutters",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": null,
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory",
            "isHidden": false
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
