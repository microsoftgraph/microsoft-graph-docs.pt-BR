---
title: Listar regras
description: Obtenha todos os objetos messageRule definidos para a caixa de entrada do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ccdf23f7fc4813bae915f673fe88ab54d15173d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511632"
---
# <a name="list-rules"></a><span data-ttu-id="0788b-103">Listar regras</span><span class="sxs-lookup"><span data-stu-id="0788b-103">List rules</span></span>

<span data-ttu-id="0788b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0788b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0788b-105">Obtenha todos os objetos [messageRule](../resources/messagerule.md) definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="0788b-105">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="0788b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0788b-106">Permissions</span></span>
<span data-ttu-id="0788b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0788b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0788b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0788b-109">Permission type</span></span>      | <span data-ttu-id="0788b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0788b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0788b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0788b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0788b-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0788b-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0788b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0788b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0788b-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0788b-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="0788b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0788b-115">Application</span></span> | <span data-ttu-id="0788b-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="0788b-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0788b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0788b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0788b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0788b-118">Optional query parameters</span></span>
<span data-ttu-id="0788b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0788b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0788b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0788b-120">Request headers</span></span>
| <span data-ttu-id="0788b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0788b-121">Name</span></span>       | <span data-ttu-id="0788b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0788b-122">Type</span></span> | <span data-ttu-id="0788b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0788b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0788b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0788b-124">Authorization</span></span>  | <span data-ttu-id="0788b-125">string</span><span class="sxs-lookup"><span data-stu-id="0788b-125">string</span></span>  | <span data-ttu-id="0788b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0788b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0788b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0788b-128">Request body</span></span>
<span data-ttu-id="0788b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0788b-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0788b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0788b-130">Response</span></span>
<span data-ttu-id="0788b-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0788b-131">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0788b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0788b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0788b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0788b-133">Request</span></span>
<span data-ttu-id="0788b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0788b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0788b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0788b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "get_messagerules"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
```
# <a name="c"></a>[<span data-ttu-id="0788b-136">C#</span><span class="sxs-lookup"><span data-stu-id="0788b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0788b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0788b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0788b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0788b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0788b-139">Java</span><span class="sxs-lookup"><span data-stu-id="0788b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0788b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0788b-140">Response</span></span>
<span data-ttu-id="0788b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0788b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
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
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
