---
title: Listar regras
description: Obtenha todos os objetos messageRule definidos para a Caixa de Entrada do usuário.
ms.openlocfilehash: 05d852171c88c519274b18a42655567f46529b9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004174"
---
# <a name="list-rules"></a><span data-ttu-id="4a062-103">Listar regras</span><span class="sxs-lookup"><span data-stu-id="4a062-103">List rules</span></span>

<span data-ttu-id="4a062-104">Obtenha todos os objetos [messageRule](../resources/messagerule.md) definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a062-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a062-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a062-105">Permissions</span></span>
<span data-ttu-id="4a062-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a062-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a062-108">Permission type</span></span>      | <span data-ttu-id="4a062-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a062-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a062-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a062-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a062-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4a062-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4a062-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a062-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a062-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4a062-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4a062-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a062-114">Application</span></span> | <span data-ttu-id="4a062-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4a062-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a062-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a062-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a062-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4a062-117">Optional query parameters</span></span>
<span data-ttu-id="4a062-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4a062-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4a062-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a062-119">Request headers</span></span>
| <span data-ttu-id="4a062-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4a062-120">Name</span></span>       | <span data-ttu-id="4a062-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a062-121">Type</span></span> | <span data-ttu-id="4a062-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a062-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4a062-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a062-123">Authorization</span></span>  | <span data-ttu-id="4a062-124">string</span><span class="sxs-lookup"><span data-stu-id="4a062-124">string</span></span>  | <span data-ttu-id="4a062-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a062-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a062-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a062-127">Request body</span></span>
<span data-ttu-id="4a062-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a062-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a062-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a062-129">Response</span></span>
<span data-ttu-id="4a062-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a062-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a062-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a062-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a062-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a062-132">Request</span></span>
<span data-ttu-id="4a062-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a062-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
```
##### <a name="response"></a><span data-ttu-id="4a062-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a062-134">Response</span></span>
<span data-ttu-id="4a062-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a062-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
