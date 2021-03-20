---
title: Listar educationClasses
description: Recupera uma lista de classes de propriedade de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5c02a27b1177e85cc00e96005faa5eb4ee3fc4d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951333"
---
# <a name="list-educationclasses"></a><span data-ttu-id="c080b-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="c080b-103">List educationClasses</span></span>

<span data-ttu-id="c080b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c080b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c080b-105">Recupera uma lista de classes de propriedade de uma escola.</span><span class="sxs-lookup"><span data-stu-id="c080b-105">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c080b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c080b-106">Permissions</span></span>
<span data-ttu-id="c080b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c080b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c080b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c080b-109">Permission type</span></span>      | <span data-ttu-id="c080b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c080b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c080b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c080b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c080b-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c080b-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c080b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c080b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c080b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c080b-114">Not supported.</span></span>  |
|<span data-ttu-id="c080b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c080b-115">Application</span></span> | <span data-ttu-id="c080b-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c080b-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c080b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c080b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c080b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c080b-118">Optional query parameters</span></span>
<span data-ttu-id="c080b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c080b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c080b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c080b-120">Request headers</span></span>
| <span data-ttu-id="c080b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c080b-121">Header</span></span>       | <span data-ttu-id="c080b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c080b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c080b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c080b-123">Authorization</span></span>  | <span data-ttu-id="c080b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c080b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c080b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c080b-126">Request body</span></span>
<span data-ttu-id="c080b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c080b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c080b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c080b-128">Response</span></span>
<span data-ttu-id="c080b-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c080b-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c080b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c080b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c080b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c080b-131">Request</span></span>
<span data-ttu-id="c080b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c080b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c080b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c080b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
# <a name="c"></a>[<span data-ttu-id="c080b-134">C#</span><span class="sxs-lookup"><span data-stu-id="c080b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c080b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c080b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c080b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c080b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c080b-137">Java</span><span class="sxs-lookup"><span data-stu-id="c080b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c080b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c080b-138">Response</span></span>
<span data-ttu-id="c080b-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c080b-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c080b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c080b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
