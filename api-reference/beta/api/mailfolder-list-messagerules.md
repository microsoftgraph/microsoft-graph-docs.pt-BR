---
title: Listar regras
description: Obtenha todos os objetos messageRule definidos para a Caixa de Entrada do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c6e800ab7a42d38b397cfcfd4426e59f4b9ae80b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984060"
---
# <a name="list-rules"></a><span data-ttu-id="5b62e-103">Listar regras</span><span class="sxs-lookup"><span data-stu-id="5b62e-103">List rules</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b62e-104">Obtenha todos os objetos [messageRule](../resources/messagerule.md) definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b62e-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b62e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b62e-105">Permissions</span></span>
<span data-ttu-id="5b62e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b62e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b62e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b62e-108">Permission type</span></span>      | <span data-ttu-id="5b62e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b62e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b62e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b62e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b62e-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5b62e-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="5b62e-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b62e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b62e-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5b62e-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="5b62e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b62e-114">Application</span></span> | <span data-ttu-id="5b62e-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="5b62e-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b62e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b62e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b62e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b62e-117">Optional query parameters</span></span>
<span data-ttu-id="5b62e-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b62e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b62e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b62e-119">Request headers</span></span>
| <span data-ttu-id="5b62e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5b62e-120">Name</span></span>       | <span data-ttu-id="5b62e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b62e-121">Type</span></span> | <span data-ttu-id="5b62e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b62e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b62e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b62e-123">Authorization</span></span>  | <span data-ttu-id="5b62e-124">string</span><span class="sxs-lookup"><span data-stu-id="5b62e-124">string</span></span>  | <span data-ttu-id="5b62e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b62e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b62e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b62e-127">Request body</span></span>
<span data-ttu-id="5b62e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b62e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5b62e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b62e-129">Response</span></span>
<span data-ttu-id="5b62e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b62e-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b62e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b62e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b62e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b62e-132">Request</span></span>
<span data-ttu-id="5b62e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b62e-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b62e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b62e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b62e-135">C#</span><span class="sxs-lookup"><span data-stu-id="5b62e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b62e-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b62e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b62e-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5b62e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5b62e-138">Java</span><span class="sxs-lookup"><span data-stu-id="5b62e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5b62e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b62e-139">Response</span></span>
<span data-ttu-id="5b62e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b62e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules",
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
<!--
{
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
