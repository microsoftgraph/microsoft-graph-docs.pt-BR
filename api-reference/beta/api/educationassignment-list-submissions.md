---
title: Listar envios
description: Listar todos os envios associados a essa atribuição. Um professor pode receber todos os envios enquanto um aluno só pode receber envios aos que estão associados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5f1d679e91974fb905c3a0ecc981fc06a49752e6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472166"
---
# <a name="list-submissions"></a><span data-ttu-id="c3fb2-104">Listar envios</span><span class="sxs-lookup"><span data-stu-id="c3fb2-104">List submissions</span></span>

<span data-ttu-id="c3fb2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3fb2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3fb2-106">Listar todos os envios associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="c3fb2-107">Um professor pode receber todos os envios enquanto um aluno só pode receber envios aos que estão associados.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-107">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3fb2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3fb2-108">Permissions</span></span>
<span data-ttu-id="c3fb2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3fb2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3fb2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3fb2-111">Permission type</span></span>      | <span data-ttu-id="c3fb2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3fb2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3fb2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3fb2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c3fb2-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3fb2-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c3fb2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3fb2-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c3fb2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-116">Not supported.</span></span>  |
|<span data-ttu-id="c3fb2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3fb2-117">Application</span></span> | <span data-ttu-id="c3fb2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-118">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3fb2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3fb2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3fb2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3fb2-120">Optional query parameters</span></span>
<span data-ttu-id="c3fb2-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3fb2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3fb2-122">Request headers</span></span>
| <span data-ttu-id="c3fb2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3fb2-123">Header</span></span>       | <span data-ttu-id="c3fb2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c3fb2-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3fb2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3fb2-125">Authorization</span></span>  | <span data-ttu-id="c3fb2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3fb2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3fb2-128">Request body</span></span>
<span data-ttu-id="c3fb2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c3fb2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3fb2-130">Response</span></span>
<span data-ttu-id="c3fb2-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-131">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3fb2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3fb2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3fb2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3fb2-133">Request</span></span>
<span data-ttu-id="c3fb2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3fb2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3fb2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
# <a name="c"></a>[<span data-ttu-id="c3fb2-136">C#</span><span class="sxs-lookup"><span data-stu-id="c3fb2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3fb2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3fb2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3fb2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3fb2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3fb2-139">Java</span><span class="sxs-lookup"><span data-stu-id="c3fb2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3fb2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3fb2-140">Response</span></span>
<span data-ttu-id="c3fb2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-141">The following is an example of the response.</span></span> 

><span data-ttu-id="c3fb2-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3fb2-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3fb2-143">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
