---
title: Obter educationSubmission
description: 'Recupere um determinado envio. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao qual o envio é atribuído pode ver e modificar o envio. Um professor tem acesso total a todos os envios. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 97cdc45c8af271d0996ea5edabf145f239162210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325147"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="02546-107">Obter educationSubmission</span><span class="sxs-lookup"><span data-stu-id="02546-107">Get educationSubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02546-108">Recupere um determinado envio.</span><span class="sxs-lookup"><span data-stu-id="02546-108">Retrieve a particular submission.</span></span> <span data-ttu-id="02546-109">Um objeto de envio representa o trabalho de um aluno para uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="02546-109">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="02546-110">Os recursos associados ao envio representam esse trabalho.</span><span class="sxs-lookup"><span data-stu-id="02546-110">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="02546-111">Somente o aluno ao qual o envio é atribuído pode ver e modificar o envio.</span><span class="sxs-lookup"><span data-stu-id="02546-111">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="02546-112">Um professor tem acesso total a todos os envios.</span><span class="sxs-lookup"><span data-stu-id="02546-112">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="02546-113">A classificação e os comentários de um professor também fazem parte desse objeto.</span><span class="sxs-lookup"><span data-stu-id="02546-113">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="02546-114">Somente os professores podem adicionar ou alterar notas e comentários.</span><span class="sxs-lookup"><span data-stu-id="02546-114">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="02546-115">Os alunos não verão a nota ou os comentários até que a atribuição tenha sido liberada.</span><span class="sxs-lookup"><span data-stu-id="02546-115">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="02546-116">As permissões básicas não incluem a classificação e o feedback, mas incluem tudo o mais.</span><span class="sxs-lookup"><span data-stu-id="02546-116">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="02546-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="02546-117">Permissions</span></span>
<span data-ttu-id="02546-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02546-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02546-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02546-120">Permission type</span></span>      | <span data-ttu-id="02546-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02546-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02546-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02546-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="02546-123">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02546-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="02546-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02546-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02546-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02546-125">Not supported.</span></span>  |
|<span data-ttu-id="02546-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02546-126">Application</span></span> | <span data-ttu-id="02546-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02546-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="02546-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02546-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02546-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02546-129">Optional query parameters</span></span>
<span data-ttu-id="02546-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02546-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02546-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02546-131">Request headers</span></span>
| <span data-ttu-id="02546-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02546-132">Header</span></span>       | <span data-ttu-id="02546-133">Valor</span><span class="sxs-lookup"><span data-stu-id="02546-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02546-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="02546-134">Authorization</span></span>  | <span data-ttu-id="02546-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02546-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02546-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02546-137">Request body</span></span>
<span data-ttu-id="02546-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02546-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="02546-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02546-139">Response</span></span>
<span data-ttu-id="02546-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02546-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02546-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02546-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02546-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02546-142">Request</span></span>
<span data-ttu-id="02546-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02546-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="02546-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="02546-144">Response</span></span>
<span data-ttu-id="02546-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02546-145">The following is an example of the response.</span></span> 

><span data-ttu-id="02546-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02546-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "feedback": {
      text: {
        "content": "Good work!",
        "contentType": "Text"
      },
      feedbackDateTime: "2014-01-01T00:00:00Z",
      feedbackBy: {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
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
        "userId": "13015"
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
