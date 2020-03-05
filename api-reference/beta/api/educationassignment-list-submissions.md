---
title: Envios de lista
description: Listar todos os envios associados a esta atribuição. Um professor pode obter todos os envios, enquanto um aluno só pode obter os envios associados a eles.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39a16e5ac1b710200b0370a74772d9c776167b2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427372"
---
# <a name="list-submissions"></a><span data-ttu-id="9bae5-104">Envios de lista</span><span class="sxs-lookup"><span data-stu-id="9bae5-104">List submissions</span></span>

<span data-ttu-id="9bae5-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9bae5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bae5-106">Listar todos os envios associados a esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="9bae5-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="9bae5-107">Um professor pode obter todos os envios, enquanto um aluno só pode obter os envios associados a eles.</span><span class="sxs-lookup"><span data-stu-id="9bae5-107">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bae5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bae5-108">Permissions</span></span>
<span data-ttu-id="9bae5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bae5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bae5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bae5-111">Permission type</span></span>      | <span data-ttu-id="9bae5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bae5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bae5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bae5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9bae5-114">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bae5-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9bae5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bae5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9bae5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bae5-116">Not supported.</span></span>  |
|<span data-ttu-id="9bae5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bae5-117">Application</span></span> | <span data-ttu-id="9bae5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bae5-118">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9bae5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bae5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9bae5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9bae5-120">Optional query parameters</span></span>
<span data-ttu-id="9bae5-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bae5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bae5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bae5-122">Request headers</span></span>
| <span data-ttu-id="9bae5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bae5-123">Header</span></span>       | <span data-ttu-id="9bae5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="9bae5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9bae5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bae5-125">Authorization</span></span>  | <span data-ttu-id="9bae5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bae5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9bae5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bae5-128">Request body</span></span>
<span data-ttu-id="9bae5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bae5-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9bae5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bae5-130">Response</span></span>
<span data-ttu-id="9bae5-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bae5-131">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9bae5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bae5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bae5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bae5-133">Request</span></span>
<span data-ttu-id="9bae5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bae5-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="9bae5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bae5-135">Response</span></span>
<span data-ttu-id="9bae5-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9bae5-136">The following is an example of the response.</span></span> 

><span data-ttu-id="9bae5-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9bae5-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9bae5-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bae5-138">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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
