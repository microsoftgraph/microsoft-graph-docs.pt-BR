---
title: Listar envios
description: Listar todos os envios associados a essa atribuição. Um professor ou um aplicativo com permissões de aplicativo pode obter todos os envios enquanto um aluno só pode receber envios aos que estão associados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7cbe965cde21b358eaa21adbdd994bb88070fbfc
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061669"
---
# <a name="list-submissions"></a><span data-ttu-id="522d0-104">Listar envios</span><span class="sxs-lookup"><span data-stu-id="522d0-104">List submissions</span></span>

<span data-ttu-id="522d0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="522d0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="522d0-106">Listar todos os envios associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="522d0-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="522d0-107">Um professor ou um aplicativo com permissões de aplicativo pode obter todos os envios enquanto um aluno só pode receber envios aos que estão associados.</span><span class="sxs-lookup"><span data-stu-id="522d0-107">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="522d0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="522d0-108">Permissions</span></span>
<span data-ttu-id="522d0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="522d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="522d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="522d0-111">Permission type</span></span>      | <span data-ttu-id="522d0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="522d0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="522d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="522d0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="522d0-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="522d0-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="522d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="522d0-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="522d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="522d0-116">Not supported.</span></span>  |
|<span data-ttu-id="522d0-117">Application\*</span><span class="sxs-lookup"><span data-stu-id="522d0-117">Application\*</span></span> | <span data-ttu-id="522d0-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="522d0-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="522d0-119">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="522d0-119">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="522d0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="522d0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="522d0-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="522d0-121">Optional query parameters</span></span>
<span data-ttu-id="522d0-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="522d0-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="522d0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="522d0-123">Request headers</span></span>
| <span data-ttu-id="522d0-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="522d0-124">Header</span></span>       | <span data-ttu-id="522d0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="522d0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="522d0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="522d0-126">Authorization</span></span>  | <span data-ttu-id="522d0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="522d0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="522d0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="522d0-129">Request body</span></span>
<span data-ttu-id="522d0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="522d0-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="522d0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="522d0-131">Response</span></span>
<span data-ttu-id="522d0-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="522d0-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="522d0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="522d0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="522d0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="522d0-134">Request</span></span>
<span data-ttu-id="522d0-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="522d0-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="522d0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="522d0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
# <a name="c"></a>[<span data-ttu-id="522d0-137">C#</span><span class="sxs-lookup"><span data-stu-id="522d0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="522d0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="522d0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="522d0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="522d0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="522d0-140">Java</span><span class="sxs-lookup"><span data-stu-id="522d0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="522d0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="522d0-141">Response</span></span>
<span data-ttu-id="522d0-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="522d0-142">The following is an example of the response.</span></span> 

><span data-ttu-id="522d0-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="522d0-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
