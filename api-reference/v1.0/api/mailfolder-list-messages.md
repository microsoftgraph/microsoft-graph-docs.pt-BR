---
title: Listar mensagens
description: Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0e04715d011d2cb4217c73b7dc234d48f38d56cb
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612462"
---
# <a name="list-messages"></a><span data-ttu-id="a9af9-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="a9af9-103">List messages</span></span>

<span data-ttu-id="a9af9-104">Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a9af9-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9af9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9af9-105">Permissions</span></span>
<span data-ttu-id="a9af9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9af9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9af9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9af9-108">Permission type</span></span>      | <span data-ttu-id="a9af9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9af9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9af9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9af9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9af9-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9af9-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a9af9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9af9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9af9-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9af9-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a9af9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9af9-114">Application</span></span> | <span data-ttu-id="a9af9-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9af9-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9af9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9af9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9af9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9af9-117">Optional query parameters</span></span>
<span data-ttu-id="a9af9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9af9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a9af9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9af9-119">Request headers</span></span>
| <span data-ttu-id="a9af9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a9af9-120">Name</span></span>       | <span data-ttu-id="a9af9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9af9-121">Type</span></span> | <span data-ttu-id="a9af9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9af9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a9af9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9af9-123">Authorization</span></span>  | <span data-ttu-id="a9af9-124">string</span><span class="sxs-lookup"><span data-stu-id="a9af9-124">string</span></span>  | <span data-ttu-id="a9af9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9af9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9af9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9af9-127">Request body</span></span>
<span data-ttu-id="a9af9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9af9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9af9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9af9-129">Response</span></span>

<span data-ttu-id="a9af9-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9af9-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9af9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9af9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9af9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9af9-132">Request</span></span>
<span data-ttu-id="a9af9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9af9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="a9af9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9af9-134">Response</span></span>
<span data-ttu-id="a9af9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9af9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a9af9-138">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="a9af9-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a9af9-139">C#</span><span class="sxs-lookup"><span data-stu-id="a9af9-139">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9af9-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9af9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
