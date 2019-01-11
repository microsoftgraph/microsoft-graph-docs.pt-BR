---
title: Obter educationSubmission
description: 'Recupere o envio de um determinado. Um objeto de envio representa trabalho student para uma atribuição. Recursos associados representam o envio isso funcione. Somente o aluno a que o envio é atribuído pode ver e modificar o envio. Um professor possui acesso total para todos os envios. '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 4eacc6ce261566afdc6d712172d35a46f9d9e595
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813360"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="6d85d-107">Obter educationSubmission</span><span class="sxs-lookup"><span data-stu-id="6d85d-107">Get educationSubmission</span></span>

> <span data-ttu-id="6d85d-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d85d-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d85d-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d85d-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d85d-110">Recupere o envio de um determinado.</span><span class="sxs-lookup"><span data-stu-id="6d85d-110">Retrieve a particular submission.</span></span> <span data-ttu-id="6d85d-111">Um objeto de envio representa trabalho student para uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="6d85d-111">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="6d85d-112">Recursos associados representam o envio isso funcione.</span><span class="sxs-lookup"><span data-stu-id="6d85d-112">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="6d85d-113">Somente o aluno a que o envio é atribuído pode ver e modificar o envio.</span><span class="sxs-lookup"><span data-stu-id="6d85d-113">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="6d85d-114">Um professor possui acesso total para todos os envios.</span><span class="sxs-lookup"><span data-stu-id="6d85d-114">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="6d85d-115">O nível e os comentários feitos durante um professor também fazem parte deste objeto.</span><span class="sxs-lookup"><span data-stu-id="6d85d-115">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="6d85d-116">Professores só podem adicionar ou alterar comentários e notas.</span><span class="sxs-lookup"><span data-stu-id="6d85d-116">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="6d85d-117">Alunos não verá o nível ou comentários até que a atribuição foi liberada.</span><span class="sxs-lookup"><span data-stu-id="6d85d-117">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="6d85d-118">As permissões básicas não incluir nível e comentários mas incluem todos os outros.</span><span class="sxs-lookup"><span data-stu-id="6d85d-118">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d85d-119">Permissions</span><span class="sxs-lookup"><span data-stu-id="6d85d-119">Permissions</span></span>
<span data-ttu-id="6d85d-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d85d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d85d-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d85d-122">Permission type</span></span>      | <span data-ttu-id="6d85d-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d85d-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d85d-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d85d-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="6d85d-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d85d-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="6d85d-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d85d-126">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6d85d-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d85d-127">Not supported.</span></span>  |
|<span data-ttu-id="6d85d-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d85d-128">Application</span></span> | <span data-ttu-id="6d85d-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d85d-129">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6d85d-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d85d-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d85d-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d85d-131">Optional query parameters</span></span>
<span data-ttu-id="6d85d-132">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d85d-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d85d-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d85d-133">Request headers</span></span>
| <span data-ttu-id="6d85d-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d85d-134">Header</span></span>       | <span data-ttu-id="6d85d-135">Valor</span><span class="sxs-lookup"><span data-stu-id="6d85d-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d85d-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d85d-136">Authorization</span></span>  | <span data-ttu-id="6d85d-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d85d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d85d-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d85d-139">Request body</span></span>
<span data-ttu-id="6d85d-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d85d-140">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6d85d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d85d-141">Response</span></span>
<span data-ttu-id="6d85d-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d85d-142">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d85d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d85d-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d85d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d85d-144">Request</span></span>
<span data-ttu-id="6d85d-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d85d-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="6d85d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d85d-146">Response</span></span>
<span data-ttu-id="6d85d-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d85d-147">The following is an example of the response.</span></span> 

><span data-ttu-id="6d85d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d85d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
