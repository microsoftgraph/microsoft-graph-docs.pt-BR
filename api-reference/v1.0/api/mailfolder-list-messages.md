---
title: Listar mensagens
description: Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5132bd1ef9bfbdd5c9926d9eff0ec91ee284d00d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128397"
---
# <a name="list-messages"></a><span data-ttu-id="52699-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="52699-103">List messages</span></span>

<span data-ttu-id="52699-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52699-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52699-105">Obtenha todas as mensagens na caixa de correio do usuário especificado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52699-105">Get all the messages in the specified user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="52699-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52699-106">Permissions</span></span>
<span data-ttu-id="52699-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52699-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52699-109">Permission type</span></span>      | <span data-ttu-id="52699-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52699-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52699-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52699-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52699-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52699-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="52699-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52699-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52699-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52699-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="52699-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52699-115">Application</span></span> | <span data-ttu-id="52699-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52699-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52699-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52699-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52699-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52699-118">Optional query parameters</span></span>
<span data-ttu-id="52699-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52699-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52699-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52699-120">Request headers</span></span>
| <span data-ttu-id="52699-121">Nome</span><span class="sxs-lookup"><span data-stu-id="52699-121">Name</span></span>       | <span data-ttu-id="52699-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="52699-122">Type</span></span> | <span data-ttu-id="52699-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="52699-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52699-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="52699-124">Authorization</span></span>  | <span data-ttu-id="52699-125">string</span><span class="sxs-lookup"><span data-stu-id="52699-125">string</span></span>  | <span data-ttu-id="52699-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52699-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52699-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52699-128">Request body</span></span>
<span data-ttu-id="52699-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52699-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52699-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52699-130">Response</span></span>

<span data-ttu-id="52699-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52699-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52699-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52699-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52699-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52699-133">Request</span></span>
<span data-ttu-id="52699-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52699-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52699-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="52699-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="c"></a>[<span data-ttu-id="52699-136">C#</span><span class="sxs-lookup"><span data-stu-id="52699-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52699-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52699-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52699-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52699-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52699-139">Java</span><span class="sxs-lookup"><span data-stu-id="52699-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52699-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="52699-140">Response</span></span>
<span data-ttu-id="52699-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52699-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "2018-02-13T03:53:55Z",
      "sentDateTime": "2018-02-13T03:53:55Z",
      "hasAttachments": true,
      "subject": "MyAnalytics | Your past week",
      "body": {
        "contentType": "html",
        "content": "<html lang=\"en\">\r\n<head></head>\r\n<body> </body>\r\n</html>\r\n"
      },
      "bodyPreview": "February 4-10, 2018\r\n\r\n\r\nHi Megan Bowen,\r\n\r\nWe've got your highlights from last week\r\n\r\n\r\n\r\nYour time\r\n\r\n\r\nEmail hours\r\n\r\n\r\n\r\n\r\n0 hrs\r\n\r\n\r\n\r\nMeeting hours\r\n\r\n\r\n\r\n\r\n12 hrs\r\n\r\n\r\n\r\n\r\nFocus hours\r\n\r\n\r\n\r\n\r\n30 hrs\r\n\r\n\r\n\r\n\r\n\r\nGoals keep you motivated. Set them"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
