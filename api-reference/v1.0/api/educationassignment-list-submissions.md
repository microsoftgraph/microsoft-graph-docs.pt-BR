---
title: Listar envios
description: Listar todos os envios associados a uma atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bfdd46767f32c552956d9b8f6aa086039e224b63
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912158"
---
# <a name="list-submissions"></a><span data-ttu-id="b34be-103">Listar envios</span><span class="sxs-lookup"><span data-stu-id="b34be-103">List submissions</span></span>

<span data-ttu-id="b34be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b34be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b34be-105">Listar todos os envios associados a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="b34be-105">List all the submissions associated with an assignment.</span></span> 

<span data-ttu-id="b34be-106">Um professor ou um aplicativo com permissões de aplicativo pode obter todos os envios enquanto um aluno só pode receber envios aos que estão associados.</span><span class="sxs-lookup"><span data-stu-id="b34be-106">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="b34be-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b34be-107">Permissions</span></span>
<span data-ttu-id="b34be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b34be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b34be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b34be-110">Permission type</span></span>      | <span data-ttu-id="b34be-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b34be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b34be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b34be-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b34be-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b34be-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b34be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b34be-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b34be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b34be-115">Not supported.</span></span>  |
|<span data-ttu-id="b34be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b34be-116">Application</span></span> | <span data-ttu-id="b34be-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b34be-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b34be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b34be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b34be-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b34be-119">Optional query parameters</span></span>
<span data-ttu-id="b34be-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b34be-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b34be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b34be-121">Request headers</span></span>
| <span data-ttu-id="b34be-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b34be-122">Header</span></span>       | <span data-ttu-id="b34be-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b34be-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b34be-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b34be-124">Authorization</span></span>  | <span data-ttu-id="b34be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b34be-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b34be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b34be-127">Request body</span></span>
<span data-ttu-id="b34be-128">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="b34be-128">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b34be-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34be-129">Response</span></span>
<span data-ttu-id="b34be-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b34be-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b34be-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b34be-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b34be-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b34be-132">Request</span></span>
<span data-ttu-id="b34be-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b34be-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions
```

### <a name="response"></a><span data-ttu-id="b34be-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34be-134">Response</span></span>
<span data-ttu-id="b34be-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b34be-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b34be-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b34be-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
            "displayName": "Shawn Hughes",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Shawn Hughes",
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
