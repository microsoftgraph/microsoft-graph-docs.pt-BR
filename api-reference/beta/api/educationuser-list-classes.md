---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: ba276c72cc34c502670d73b70d10958954ccd691
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859815"
---
# <a name="list-classes"></a><span data-ttu-id="0c694-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="0c694-104">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c694-105">Recupere uma lista de objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="0c694-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="0c694-106">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="0c694-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="0c694-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c694-107">Permissions</span></span>
<span data-ttu-id="0c694-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c694-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c694-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c694-110">Permission type</span></span>      | <span data-ttu-id="0c694-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c694-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c694-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c694-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c694-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0c694-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="0c694-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c694-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c694-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c694-115">Not supported.</span></span>  |
|<span data-ttu-id="0c694-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c694-116">Application</span></span> | <span data-ttu-id="0c694-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c694-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c694-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c694-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0c694-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0c694-119">Optional query parameters</span></span>
<span data-ttu-id="0c694-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0c694-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c694-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c694-121">Request headers</span></span>
| <span data-ttu-id="0c694-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c694-122">Header</span></span>       | <span data-ttu-id="0c694-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0c694-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c694-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c694-124">Authorization</span></span>  | <span data-ttu-id="0c694-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c694-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c694-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c694-127">Request body</span></span>
<span data-ttu-id="0c694-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c694-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0c694-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c694-129">Response</span></span>
<span data-ttu-id="0c694-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c694-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c694-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c694-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c694-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c694-132">Request</span></span>
<span data-ttu-id="0c694-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c694-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c694-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c694-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c694-135">C#</span><span class="sxs-lookup"><span data-stu-id="0c694-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c694-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c694-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c694-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0c694-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c694-138">Java</span><span class="sxs-lookup"><span data-stu-id="0c694-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0c694-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c694-139">Response</span></span>
<span data-ttu-id="0c694-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c694-140">The following is an example of the response.</span></span> 

><span data-ttu-id="0c694-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c694-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
