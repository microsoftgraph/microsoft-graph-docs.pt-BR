---
title: Listar mensagens
description: Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 879e6a5b32e20acbc16c6195436678f42045870f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033038"
---
# <a name="list-messages"></a><span data-ttu-id="fca0b-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="fca0b-103">List messages</span></span>

<span data-ttu-id="fca0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fca0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fca0b-105">Obtenha todas as mensagens na caixa de correio do usuário especificado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fca0b-105">Get all the messages in the specified user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="fca0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fca0b-106">Permissions</span></span>
<span data-ttu-id="fca0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fca0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fca0b-109">Permission type</span></span>      | <span data-ttu-id="fca0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fca0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fca0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fca0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fca0b-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fca0b-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fca0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fca0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca0b-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fca0b-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fca0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fca0b-115">Application</span></span> | <span data-ttu-id="fca0b-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fca0b-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fca0b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fca0b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fca0b-118">Optional query parameters</span></span>
<span data-ttu-id="fca0b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fca0b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fca0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fca0b-120">Request headers</span></span>
| <span data-ttu-id="fca0b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fca0b-121">Name</span></span>       | <span data-ttu-id="fca0b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fca0b-122">Type</span></span> | <span data-ttu-id="fca0b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fca0b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fca0b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fca0b-124">Authorization</span></span>  | <span data-ttu-id="fca0b-125">string</span><span class="sxs-lookup"><span data-stu-id="fca0b-125">string</span></span>  | <span data-ttu-id="fca0b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fca0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fca0b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fca0b-128">Request body</span></span>
<span data-ttu-id="fca0b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fca0b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca0b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca0b-130">Response</span></span>

<span data-ttu-id="fca0b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fca0b-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fca0b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fca0b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fca0b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fca0b-133">Request</span></span>
<span data-ttu-id="fca0b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fca0b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fca0b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fca0b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="c"></a>[<span data-ttu-id="fca0b-136">C#</span><span class="sxs-lookup"><span data-stu-id="fca0b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fca0b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fca0b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fca0b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fca0b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fca0b-139">Java</span><span class="sxs-lookup"><span data-stu-id="fca0b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fca0b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca0b-140">Response</span></span>
<span data-ttu-id="fca0b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fca0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
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

