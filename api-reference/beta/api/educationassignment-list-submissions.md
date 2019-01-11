---
title: Envios de lista
description: Liste todos os envios associados a essa atribuição. Um professor pode obter todos os envios enquanto um estudante só pode obter envios que eles estão associados.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 0b807a1b19bdb47e3b184ffdce4a15b38740c574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883205"
---
# <a name="list-submissions"></a><span data-ttu-id="92c97-104">Envios de lista</span><span class="sxs-lookup"><span data-stu-id="92c97-104">List submissions</span></span>

> <span data-ttu-id="92c97-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92c97-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92c97-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92c97-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92c97-107">Liste todos os envios associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="92c97-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="92c97-108">Um professor pode obter todos os envios enquanto um estudante só pode obter envios que eles estão associados.</span><span class="sxs-lookup"><span data-stu-id="92c97-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="92c97-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="92c97-109">Permissions</span></span>
<span data-ttu-id="92c97-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92c97-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92c97-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92c97-112">Permission type</span></span>      | <span data-ttu-id="92c97-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92c97-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92c97-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92c97-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="92c97-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c97-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="92c97-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92c97-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="92c97-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92c97-117">Not supported.</span></span>  |
|<span data-ttu-id="92c97-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92c97-118">Application</span></span> | <span data-ttu-id="92c97-119">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="92c97-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="92c97-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92c97-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92c97-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92c97-121">Optional query parameters</span></span>
<span data-ttu-id="92c97-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92c97-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92c97-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92c97-123">Request headers</span></span>
| <span data-ttu-id="92c97-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92c97-124">Header</span></span>       | <span data-ttu-id="92c97-125">Valor</span><span class="sxs-lookup"><span data-stu-id="92c97-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92c97-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="92c97-126">Authorization</span></span>  | <span data-ttu-id="92c97-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92c97-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92c97-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92c97-129">Request body</span></span>
<span data-ttu-id="92c97-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92c97-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="92c97-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="92c97-131">Response</span></span>
<span data-ttu-id="92c97-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92c97-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92c97-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92c97-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92c97-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92c97-134">Request</span></span>
<span data-ttu-id="92c97-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92c97-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="92c97-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92c97-136">Response</span></span>
<span data-ttu-id="92c97-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92c97-137">The following is an example of the response.</span></span> 

><span data-ttu-id="92c97-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="92c97-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="92c97-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92c97-139">All of the properties will be returned from an actual call.</span></span>

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
