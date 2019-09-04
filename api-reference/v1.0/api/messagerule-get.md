---
title: Obter regra
description: Obtenha as propriedades e as relações de um objeto messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: aed60b2227416f34e01752ce2267d342524a6c75
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730229"
---
# <a name="get-rule"></a><span data-ttu-id="5f100-103">Obter regra</span><span class="sxs-lookup"><span data-stu-id="5f100-103">Get rule</span></span>


<span data-ttu-id="5f100-104">Obtenha as propriedades e as relações de um objeto [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="5f100-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="5f100-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f100-105">Permissions</span></span>
<span data-ttu-id="5f100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f100-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f100-108">Permission type</span></span>      | <span data-ttu-id="5f100-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f100-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f100-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f100-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f100-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5f100-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="5f100-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f100-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f100-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5f100-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="5f100-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f100-114">Application</span></span> | <span data-ttu-id="5f100-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5f100-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f100-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f100-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5f100-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f100-117">Optional query parameters</span></span>
<span data-ttu-id="5f100-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f100-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f100-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f100-119">Request headers</span></span>
| <span data-ttu-id="5f100-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5f100-120">Name</span></span>      |<span data-ttu-id="5f100-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f100-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f100-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f100-122">Authorization</span></span>  | <span data-ttu-id="5f100-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f100-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5f100-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f100-125">Request body</span></span>
<span data-ttu-id="5f100-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f100-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5f100-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f100-127">Response</span></span>
<span data-ttu-id="5f100-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f100-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f100-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f100-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f100-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f100-130">Request</span></span>
<span data-ttu-id="5f100-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f100-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5f100-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f100-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f100-133">C#</span><span class="sxs-lookup"><span data-stu-id="5f100-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f100-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f100-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f100-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5f100-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5f100-136">Java</span><span class="sxs-lookup"><span data-stu-id="5f100-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5f100-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f100-137">Response</span></span>
<span data-ttu-id="5f100-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f100-138">Here is an example of the response.</span></span> <span data-ttu-id="5f100-139">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="5f100-139">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="5f100-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f100-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
