---
title: Listar classes
description: 'Recupere uma lista de todos os objetos de classe. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 66a2f3dce7bac5a121244876d69051e60703b9cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007510"
---
# <a name="list-classes"></a><span data-ttu-id="790f4-103">Listar classes</span><span class="sxs-lookup"><span data-stu-id="790f4-103">List classes</span></span>

<span data-ttu-id="790f4-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="790f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="790f4-105">Recupere uma lista de todos os objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="790f4-105">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="790f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="790f4-106">Permissions</span></span>
<span data-ttu-id="790f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="790f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="790f4-109">Permission type</span></span>      | <span data-ttu-id="790f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="790f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="790f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="790f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="790f4-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="790f4-112">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="790f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="790f4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="790f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="790f4-114">Not supported.</span></span>  |
|<span data-ttu-id="790f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="790f4-115">Application</span></span> | <span data-ttu-id="790f4-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="790f4-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="790f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="790f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="790f4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="790f4-118">Optional query parameters</span></span>
<span data-ttu-id="790f4-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="790f4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="790f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="790f4-120">Request headers</span></span>
| <span data-ttu-id="790f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="790f4-121">Header</span></span>       | <span data-ttu-id="790f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="790f4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="790f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="790f4-123">Authorization</span></span>  | <span data-ttu-id="790f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="790f4-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="790f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="790f4-126">Request body</span></span>
<span data-ttu-id="790f4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="790f4-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="790f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="790f4-128">Response</span></span>
<span data-ttu-id="790f4-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="790f4-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="790f4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="790f4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="790f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="790f4-131">Request</span></span>
<span data-ttu-id="790f4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="790f4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="790f4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="790f4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes
```
# <a name="c"></a>[<span data-ttu-id="790f4-134">C#</span><span class="sxs-lookup"><span data-stu-id="790f4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="790f4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="790f4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="790f4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="790f4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="790f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="790f4-137">Response</span></span>
<span data-ttu-id="790f4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="790f4-138">The following is an example of the response.</span></span> 

><span data-ttu-id="790f4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="790f4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


