---
title: Listar mailFolders
description: 'Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. '
author: abheek-das
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 707daff5e3043d10c038343967fa421875132788
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629522"
---
# <a name="list-mailfolders"></a><span data-ttu-id="fc0a7-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="fc0a7-103">List mailFolders</span></span>

<span data-ttu-id="fc0a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc0a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc0a7-105">Obter o conjunto de pastas de email diretamente sob a pasta raiz do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-105">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="fc0a7-106">O conjunto retornado inclui todas as [pastas de pesquisa de email](../resources/mailsearchfolder.md) diretamente sob a raiz.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-106">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

<span data-ttu-id="fc0a7-107">Por padrão, esta operação não retorna pastas ocultas.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-107">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="fc0a7-108">Use um parâmetro de consulta _includeHiddenFolders_ para incluí-los na resposta.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-108">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc0a7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc0a7-109">Permissions</span></span>
<span data-ttu-id="fc0a7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc0a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc0a7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc0a7-112">Permission type</span></span>      | <span data-ttu-id="fc0a7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc0a7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc0a7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc0a7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fc0a7-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc0a7-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fc0a7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc0a7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc0a7-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc0a7-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fc0a7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc0a7-118">Application</span></span> | <span data-ttu-id="fc0a7-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc0a7-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc0a7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc0a7-120">HTTP request</span></span>

<span data-ttu-id="fc0a7-121">Para obter todas as pastas de email na caixa de correio do usuário especificado, exceto aquelas que estão ocultas:</span><span class="sxs-lookup"><span data-stu-id="fc0a7-121">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="fc0a7-122">Para incluir pastas de email _ocultas_ na resposta:</span><span class="sxs-lookup"><span data-stu-id="fc0a7-122">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc0a7-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc0a7-123">Optional query parameters</span></span>
<span data-ttu-id="fc0a7-124">Para retornar uma lista de todas as mailFolders, incluindo aquelas que estão ocultas (sua propriedade **isHidden** é verdadeira), no URL da solicitação, especifique o `includeHiddenFolders` parâmetro de consulta como `true`, conforme mostrado na seção de [solicitação HTTP](#http-request).</span><span class="sxs-lookup"><span data-stu-id="fc0a7-124">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="fc0a7-125">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fc0a7-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0a7-126">Request headers</span></span>
| <span data-ttu-id="fc0a7-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc0a7-127">Header</span></span>       | <span data-ttu-id="fc0a7-128">Valor</span><span class="sxs-lookup"><span data-stu-id="fc0a7-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc0a7-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc0a7-129">Authorization</span></span>  | <span data-ttu-id="fc0a7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc0a7-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc0a7-132">Content-Type</span></span>   | <span data-ttu-id="fc0a7-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fc0a7-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc0a7-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0a7-134">Request body</span></span>
<span data-ttu-id="fc0a7-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc0a7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc0a7-136">Response</span></span>

<span data-ttu-id="fc0a7-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-137">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="fc0a7-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc0a7-138">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="fc0a7-139">Exemplo 1: Listar pastas de email na caixa de correio do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="fc0a7-139">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="fc0a7-140">Este exemplo inclui um objeto **mailSearchFolder** na resposta.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-140">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="fc0a7-141">A pasta de pesquisa de email é uma pasta filho na caixa de entrada com o nome de exibição "Resumos semanais".</span><span class="sxs-lookup"><span data-stu-id="fc0a7-141">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="fc0a7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0a7-142">Request</span></span>
<span data-ttu-id="fc0a7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc0a7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc0a7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="fc0a7-145">C#</span><span class="sxs-lookup"><span data-stu-id="fc0a7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc0a7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc0a7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc0a7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc0a7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc0a7-148">Java</span><span class="sxs-lookup"><span data-stu-id="fc0a7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc0a7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc0a7-149">Response</span></span>
<span data-ttu-id="fc0a7-150">Aqui está um exemplo de resposta que inclui uma **mailSearchFolder** que é uma pasta filho na Caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-150">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="fc0a7-151">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fc0a7-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-152">All of the properties will be returned from an actual call.</span></span>

><span data-ttu-id="fc0a7-153">**Observação:** O objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
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
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        }
    ]
}
```

### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="fc0a7-154">Exemplo 2: incluir pastas ocultas na caixa de correio do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="fc0a7-154">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="fc0a7-155">O próximo exemplo usa o parâmetro de consulta `includeHiddenFolders` para obter uma lista de pastas de email, incluindo pastas de email ocultas.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-155">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="fc0a7-156">A resposta inclui a pasta "Emails secundários" que tem a **isHidden** definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-156">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="fc0a7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0a7-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```

#### <a name="response"></a><span data-ttu-id="fc0a7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc0a7-158">Response</span></span>
<span data-ttu-id="fc0a7-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-159">Here is an example of the response.</span></span>

><span data-ttu-id="fc0a7-160">**Observação:** O objeto de resposta mostrado aqui é reduzido para facilitar a leitura e não inclui todas as pastas padrões em uma caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="fc0a7-160">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
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
