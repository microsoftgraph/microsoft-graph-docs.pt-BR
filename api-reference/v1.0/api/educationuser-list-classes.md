---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4cc312917f93a4f3eaf2fe8ae0541645de349149
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275996"
---
# <a name="list-classes"></a><span data-ttu-id="d3bbb-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="d3bbb-104">List classes</span></span>

<span data-ttu-id="d3bbb-105">Recupere uma lista de objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="d3bbb-106">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="d3bbb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3bbb-107">Permissions</span></span>
<span data-ttu-id="d3bbb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3bbb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3bbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3bbb-110">Permission type</span></span>      | <span data-ttu-id="d3bbb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3bbb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3bbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3bbb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d3bbb-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d3bbb-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="d3bbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3bbb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d3bbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-115">Not supported.</span></span>  |
|<span data-ttu-id="d3bbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3bbb-116">Application</span></span> | <span data-ttu-id="d3bbb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3bbb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d3bbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3bbb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3bbb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3bbb-119">Optional query parameters</span></span>
<span data-ttu-id="d3bbb-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3bbb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3bbb-121">Request headers</span></span>
| <span data-ttu-id="d3bbb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3bbb-122">Header</span></span>       | <span data-ttu-id="d3bbb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d3bbb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3bbb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3bbb-124">Authorization</span></span>  | <span data-ttu-id="d3bbb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3bbb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3bbb-127">Request body</span></span>
<span data-ttu-id="d3bbb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d3bbb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3bbb-129">Response</span></span>
<span data-ttu-id="d3bbb-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3bbb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3bbb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3bbb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3bbb-132">Request</span></span>
<span data-ttu-id="d3bbb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="d3bbb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3bbb-134">Response</span></span>
<span data-ttu-id="d3bbb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="d3bbb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3bbb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3bbb-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d3bbb-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3bbb-139">C#</span><span class="sxs-lookup"><span data-stu-id="d3bbb-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_classes-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3bbb-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3bbb-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_classes-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3bbb-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d3bbb-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_classes-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationuser-list-classes.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationuser-list-classes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationuser-list-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
