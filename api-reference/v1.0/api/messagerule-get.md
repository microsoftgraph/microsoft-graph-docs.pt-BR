---
title: Obter regra
description: Obtenha as propriedades e as relações de um objeto messageRule.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2472b52089e230436a6a117535e0a13576586efa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054543"
---
# <a name="get-rule"></a><span data-ttu-id="94807-103">Obter regra</span><span class="sxs-lookup"><span data-stu-id="94807-103">Get rule</span></span>

<span data-ttu-id="94807-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94807-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="94807-105">Obtenha as propriedades e as relações de um objeto [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="94807-105">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="94807-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94807-106">Permissions</span></span>
<span data-ttu-id="94807-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94807-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94807-109">Permission type</span></span>      | <span data-ttu-id="94807-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94807-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94807-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94807-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94807-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="94807-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="94807-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94807-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94807-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="94807-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="94807-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94807-115">Application</span></span> | <span data-ttu-id="94807-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="94807-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="94807-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94807-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94807-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94807-118">Optional query parameters</span></span>
<span data-ttu-id="94807-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94807-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94807-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94807-120">Request headers</span></span>
| <span data-ttu-id="94807-121">Nome</span><span class="sxs-lookup"><span data-stu-id="94807-121">Name</span></span>      |<span data-ttu-id="94807-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="94807-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94807-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94807-123">Authorization</span></span>  | <span data-ttu-id="94807-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94807-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="94807-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94807-126">Request body</span></span>
<span data-ttu-id="94807-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94807-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94807-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94807-128">Response</span></span>
<span data-ttu-id="94807-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94807-129">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94807-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94807-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94807-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94807-131">Request</span></span>
<span data-ttu-id="94807-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94807-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94807-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="94807-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
# <a name="c"></a>[<span data-ttu-id="94807-134">C#</span><span class="sxs-lookup"><span data-stu-id="94807-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94807-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94807-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94807-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94807-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94807-137">Java</span><span class="sxs-lookup"><span data-stu-id="94807-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94807-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94807-138">Response</span></span>
<span data-ttu-id="94807-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94807-139">Here is an example of the response.</span></span> <span data-ttu-id="94807-140">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="94807-140">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="94807-141">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94807-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
