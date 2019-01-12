---
title: Envios de lista
description: Liste todos os envios associados a essa atribuição. Um professor pode obter todos os envios enquanto um estudante só pode obter envios que eles estão associados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2a4de863b69de420e89a9272e532fa889486fc22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915183"
---
# <a name="list-submissions"></a><span data-ttu-id="5163f-104">Envios de lista</span><span class="sxs-lookup"><span data-stu-id="5163f-104">List submissions</span></span>

> <span data-ttu-id="5163f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5163f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5163f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5163f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5163f-107">Liste todos os envios associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="5163f-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="5163f-108">Um professor pode obter todos os envios enquanto um estudante só pode obter envios que eles estão associados.</span><span class="sxs-lookup"><span data-stu-id="5163f-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="5163f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="5163f-109">Permissions</span></span>
<span data-ttu-id="5163f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5163f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5163f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5163f-112">Permission type</span></span>      | <span data-ttu-id="5163f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5163f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5163f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5163f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="5163f-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5163f-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5163f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5163f-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5163f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5163f-117">Not supported.</span></span>  |
|<span data-ttu-id="5163f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5163f-118">Application</span></span> | <span data-ttu-id="5163f-119">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="5163f-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5163f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5163f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5163f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5163f-121">Optional query parameters</span></span>
<span data-ttu-id="5163f-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5163f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5163f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5163f-123">Request headers</span></span>
| <span data-ttu-id="5163f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5163f-124">Header</span></span>       | <span data-ttu-id="5163f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5163f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5163f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5163f-126">Authorization</span></span>  | <span data-ttu-id="5163f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5163f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5163f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5163f-129">Request body</span></span>
<span data-ttu-id="5163f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5163f-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5163f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5163f-131">Response</span></span>
<span data-ttu-id="5163f-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5163f-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5163f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5163f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5163f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5163f-134">Request</span></span>
<span data-ttu-id="5163f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5163f-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="5163f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5163f-136">Response</span></span>
<span data-ttu-id="5163f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5163f-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5163f-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5163f-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5163f-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5163f-139">All of the properties will be returned from an actual call.</span></span>

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
      "feedback": {
        "text": {
          "content": "Good work!",
          "contentType": "Text"
        },
        "feedbackDateTime": "2014-01-01T00:00:00Z",
        "feedbackBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "@odata.type": "microsoft.graph.educationFeedback"
        },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
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
<!-- {
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
