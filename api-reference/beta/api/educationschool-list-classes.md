---
title: Listar educationClasses
description: Recupera uma lista de classes de propriedade de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9f1c1fc65df83e422ab939822f794ca0a93e43ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425405"
---
# <a name="list-educationclasses"></a><span data-ttu-id="c0054-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="c0054-103">List educationClasses</span></span>

<span data-ttu-id="c0054-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c0054-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0054-105">Recupera uma lista de classes de propriedade de uma escola.</span><span class="sxs-lookup"><span data-stu-id="c0054-105">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0054-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0054-106">Permissions</span></span>
<span data-ttu-id="c0054-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0054-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0054-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0054-109">Permission type</span></span>      | <span data-ttu-id="c0054-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0054-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0054-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0054-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0054-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c0054-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c0054-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0054-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0054-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0054-114">Not supported.</span></span>  |
|<span data-ttu-id="c0054-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0054-115">Application</span></span> | <span data-ttu-id="c0054-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0054-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c0054-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0054-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0054-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0054-118">Optional query parameters</span></span>
<span data-ttu-id="c0054-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0054-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0054-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0054-120">Request headers</span></span>
| <span data-ttu-id="c0054-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0054-121">Header</span></span>       | <span data-ttu-id="c0054-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0054-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0054-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0054-123">Authorization</span></span>  | <span data-ttu-id="c0054-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0054-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0054-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0054-126">Request body</span></span>
<span data-ttu-id="c0054-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0054-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c0054-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0054-128">Response</span></span>
<span data-ttu-id="c0054-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0054-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0054-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0054-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0054-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0054-131">Request</span></span>
<span data-ttu-id="c0054-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0054-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0054-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0054-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
# <a name="c"></a>[<span data-ttu-id="c0054-134">C#</span><span class="sxs-lookup"><span data-stu-id="c0054-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0054-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0054-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0054-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0054-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0054-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0054-137">Response</span></span>
<span data-ttu-id="c0054-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0054-138">The following is an example of the response.</span></span> 

><span data-ttu-id="c0054-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0054-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
