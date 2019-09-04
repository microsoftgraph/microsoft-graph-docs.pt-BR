---
title: Listar classes
description: 'Recupere uma lista de todos os objetos de classe. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e2b6dc82aa56481f7ca381382f6f26fe9a2b9820
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720435"
---
# <a name="list-classes"></a><span data-ttu-id="0befe-103">Listar classes</span><span class="sxs-lookup"><span data-stu-id="0befe-103">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0befe-104">Recupere uma lista de todos os objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="0befe-104">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0befe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0befe-105">Permissions</span></span>
<span data-ttu-id="0befe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0befe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0befe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0befe-108">Permission type</span></span>      | <span data-ttu-id="0befe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0befe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0befe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0befe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0befe-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0befe-111">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="0befe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0befe-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0befe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0befe-113">Not supported.</span></span>  |
|<span data-ttu-id="0befe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0befe-114">Application</span></span> | <span data-ttu-id="0befe-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0befe-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0befe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0befe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0befe-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0befe-117">Optional query parameters</span></span>
<span data-ttu-id="0befe-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0befe-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0befe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0befe-119">Request headers</span></span>
| <span data-ttu-id="0befe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0befe-120">Header</span></span>       | <span data-ttu-id="0befe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0befe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0befe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0befe-122">Authorization</span></span>  | <span data-ttu-id="0befe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0befe-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="0befe-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0befe-125">Request body</span></span>
<span data-ttu-id="0befe-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0befe-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0befe-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0befe-127">Response</span></span>
<span data-ttu-id="0befe-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0befe-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0befe-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0befe-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0befe-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0befe-130">Request</span></span>
<span data-ttu-id="0befe-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0befe-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0befe-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0befe-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0befe-133">C#</span><span class="sxs-lookup"><span data-stu-id="0befe-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0befe-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0befe-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0befe-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0befe-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0befe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0befe-136">Response</span></span>
<span data-ttu-id="0befe-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0befe-137">The following is an example of the response.</span></span> 

><span data-ttu-id="0befe-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0befe-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
