---
title: Listar educationClasses
description: Recupera uma lista de classes de propriedade de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bcc5601e321217b862909d5709b679956e2005fc
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721009"
---
# <a name="list-educationclasses"></a><span data-ttu-id="89ede-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="89ede-103">List educationClasses</span></span>

<span data-ttu-id="89ede-104">Recupera uma lista de classes de propriedade de uma escola.</span><span class="sxs-lookup"><span data-stu-id="89ede-104">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ede-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="89ede-105">Permissions</span></span>
<span data-ttu-id="89ede-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ede-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ede-108">Permission type</span></span>      | <span data-ttu-id="89ede-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89ede-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ede-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ede-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="89ede-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="89ede-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="89ede-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89ede-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="89ede-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ede-113">Not supported.</span></span>  |
|<span data-ttu-id="89ede-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89ede-114">Application</span></span> | <span data-ttu-id="89ede-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ede-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="89ede-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ede-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89ede-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89ede-117">Optional query parameters</span></span>
<span data-ttu-id="89ede-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="89ede-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89ede-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89ede-119">Request headers</span></span>
| <span data-ttu-id="89ede-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89ede-120">Header</span></span>       | <span data-ttu-id="89ede-121">Valor</span><span class="sxs-lookup"><span data-stu-id="89ede-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89ede-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ede-122">Authorization</span></span>  | <span data-ttu-id="89ede-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ede-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89ede-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ede-125">Request body</span></span>
<span data-ttu-id="89ede-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89ede-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="89ede-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ede-127">Response</span></span>
<span data-ttu-id="89ede-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ede-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89ede-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89ede-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89ede-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89ede-130">Request</span></span>
<span data-ttu-id="89ede-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89ede-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89ede-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="89ede-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89ede-133">C#</span><span class="sxs-lookup"><span data-stu-id="89ede-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89ede-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89ede-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89ede-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="89ede-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89ede-136">Java</span><span class="sxs-lookup"><span data-stu-id="89ede-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="89ede-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ede-137">Response</span></span>
<span data-ttu-id="89ede-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89ede-138">The following is an example of the response.</span></span> 

><span data-ttu-id="89ede-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89ede-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
