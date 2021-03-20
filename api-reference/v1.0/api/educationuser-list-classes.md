---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 34676757c10aef8cabae8b784172767a1f72e9f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941694"
---
# <a name="list-classes"></a><span data-ttu-id="50b6a-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="50b6a-104">List classes</span></span>

<span data-ttu-id="50b6a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50b6a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50b6a-106">Recupere uma lista de objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="50b6a-106">Retrieve a list of class objects.</span></span> <span data-ttu-id="50b6a-107">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="50b6a-107">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="50b6a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="50b6a-108">Permissions</span></span>
<span data-ttu-id="50b6a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50b6a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b6a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50b6a-111">Permission type</span></span>      | <span data-ttu-id="50b6a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50b6a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50b6a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50b6a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="50b6a-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="50b6a-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="50b6a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50b6a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="50b6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50b6a-116">Not supported.</span></span>  |
|<span data-ttu-id="50b6a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50b6a-117">Application</span></span> | <span data-ttu-id="50b6a-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b6a-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="50b6a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50b6a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50b6a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50b6a-120">Optional query parameters</span></span>
<span data-ttu-id="50b6a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50b6a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50b6a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50b6a-122">Request headers</span></span>
| <span data-ttu-id="50b6a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50b6a-123">Header</span></span>       | <span data-ttu-id="50b6a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="50b6a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50b6a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="50b6a-125">Authorization</span></span>  | <span data-ttu-id="50b6a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50b6a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50b6a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50b6a-128">Request body</span></span>
<span data-ttu-id="50b6a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50b6a-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="50b6a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="50b6a-130">Response</span></span>
<span data-ttu-id="50b6a-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50b6a-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50b6a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50b6a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50b6a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50b6a-133">Request</span></span>
<span data-ttu-id="50b6a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50b6a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50b6a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="50b6a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/classes
```
# <a name="c"></a>[<span data-ttu-id="50b6a-136">C#</span><span class="sxs-lookup"><span data-stu-id="50b6a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50b6a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50b6a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50b6a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50b6a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50b6a-139">Java</span><span class="sxs-lookup"><span data-stu-id="50b6a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50b6a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="50b6a-140">Response</span></span>
<span data-ttu-id="50b6a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50b6a-141">The following is an example of the response.</span></span> 

><span data-ttu-id="50b6a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50b6a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
