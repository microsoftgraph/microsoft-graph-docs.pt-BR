---
title: Listar mensagens
description: Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).
ms.openlocfilehash: 861d56850a8a4a4a167540b221bd94b7b8e62ae0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003572"
---
# <a name="list-messages"></a><span data-ttu-id="3478c-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="3478c-103">List messages</span></span>

<span data-ttu-id="3478c-104">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="3478c-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="3478c-105">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="3478c-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="3478c-106">Há dois cenários onde um aplicativo pode obter mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="3478c-106">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="3478c-107">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="3478c-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="3478c-108">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de email com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="3478c-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="3478c-109">Consulte os [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="3478c-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="3478c-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="3478c-110">Permissions</span></span>
<span data-ttu-id="3478c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3478c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3478c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3478c-113">Permission type</span></span>      | <span data-ttu-id="3478c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3478c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3478c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3478c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3478c-116">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3478c-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3478c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3478c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3478c-118">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3478c-118">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3478c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3478c-119">Application</span></span> | <span data-ttu-id="3478c-120">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3478c-120">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3478c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3478c-121">HTTP request</span></span>

<span data-ttu-id="3478c-122">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="3478c-122">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="3478c-123">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="3478c-123">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3478c-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3478c-124">Optional query parameters</span></span>
<span data-ttu-id="3478c-125">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3478c-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3478c-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3478c-126">Request headers</span></span>
| <span data-ttu-id="3478c-127">Nome</span><span class="sxs-lookup"><span data-stu-id="3478c-127">Name</span></span>       | <span data-ttu-id="3478c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="3478c-128">Type</span></span> | <span data-ttu-id="3478c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="3478c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3478c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="3478c-130">Authorization</span></span>  | <span data-ttu-id="3478c-131">string</span><span class="sxs-lookup"><span data-stu-id="3478c-131">string</span></span>  | <span data-ttu-id="3478c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3478c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3478c-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="3478c-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="3478c-135">string</span><span class="sxs-lookup"><span data-stu-id="3478c-135">string</span></span> | <span data-ttu-id="3478c-136">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="3478c-136">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="3478c-137">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="3478c-137">Values can be "text" or "html".</span></span> <span data-ttu-id="3478c-138">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="3478c-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="3478c-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3478c-139">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3478c-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3478c-140">Request body</span></span>
<span data-ttu-id="3478c-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3478c-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3478c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3478c-142">Response</span></span>

<span data-ttu-id="3478c-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3478c-143">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="3478c-144">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="3478c-144">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="3478c-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3478c-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3478c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3478c-146">Request</span></span>
<span data-ttu-id="3478c-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3478c-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="3478c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3478c-148">Response</span></span>
<span data-ttu-id="3478c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3478c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
