---
title: Obter educationSubmission
description: 'Recupere um determinado envio. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao qual o envio é atribuído pode ver e modificar o envio. Um professor tem acesso total a todos os envios. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4b07b2c76fc03854b6e296d6869b4af7e05e7dd3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007333"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="2770f-107">Obter educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2770f-107">Get educationSubmission</span></span>

<span data-ttu-id="2770f-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2770f-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2770f-109">Recupere um determinado envio.</span><span class="sxs-lookup"><span data-stu-id="2770f-109">Retrieve a particular submission.</span></span> <span data-ttu-id="2770f-110">Um objeto de envio representa o trabalho de um aluno para uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="2770f-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="2770f-111">Os recursos associados ao envio representam esse trabalho.</span><span class="sxs-lookup"><span data-stu-id="2770f-111">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="2770f-112">Somente o aluno ao qual o envio é atribuído pode ver e modificar o envio.</span><span class="sxs-lookup"><span data-stu-id="2770f-112">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="2770f-113">Um professor tem acesso total a todos os envios.</span><span class="sxs-lookup"><span data-stu-id="2770f-113">A teacher has full access to all submissions.</span></span>

<span data-ttu-id="2770f-114">A classificação e os comentários de um professor fazem parte do [educationOutcome](../resources/educationoutcome.md) associado a este objeto.</span><span class="sxs-lookup"><span data-stu-id="2770f-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="2770f-115">Somente os professores podem adicionar ou alterar notas e comentários.</span><span class="sxs-lookup"><span data-stu-id="2770f-115">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="2770f-116">Os alunos não verão a nota ou os comentários até que a atribuição tenha sido liberada.</span><span class="sxs-lookup"><span data-stu-id="2770f-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="2770f-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="2770f-117">Permissions</span></span>
<span data-ttu-id="2770f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2770f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2770f-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2770f-120">Permission type</span></span>      | <span data-ttu-id="2770f-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2770f-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2770f-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2770f-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="2770f-123">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2770f-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="2770f-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2770f-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2770f-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2770f-125">Not supported.</span></span>  |
|<span data-ttu-id="2770f-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2770f-126">Application</span></span> | <span data-ttu-id="2770f-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2770f-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2770f-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2770f-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2770f-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2770f-129">Optional query parameters</span></span>
<span data-ttu-id="2770f-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2770f-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2770f-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2770f-131">Request headers</span></span>
| <span data-ttu-id="2770f-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2770f-132">Header</span></span>       | <span data-ttu-id="2770f-133">Valor</span><span class="sxs-lookup"><span data-stu-id="2770f-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2770f-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="2770f-134">Authorization</span></span>  | <span data-ttu-id="2770f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2770f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2770f-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2770f-137">Request body</span></span>
<span data-ttu-id="2770f-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2770f-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2770f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2770f-139">Response</span></span>
<span data-ttu-id="2770f-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2770f-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2770f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2770f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2770f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2770f-142">Request</span></span>
<span data-ttu-id="2770f-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2770f-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="2770f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2770f-144">Response</span></span>
<span data-ttu-id="2770f-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2770f-145">The following is an example of the response.</span></span> 

><span data-ttu-id="2770f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2770f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


