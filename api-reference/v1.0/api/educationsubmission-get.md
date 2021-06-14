---
title: Obter educationSubmission
description: 'Recupere um envio específico. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao que o envio é atribuído pode ver e modificar o envio. Um professor ou aplicativo com permissões de aplicativo tem acesso total a todos os envios. '
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3188fd2c1bb9643cb9ba8f94621cd08067572b71
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912228"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="c2353-107">Obter educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c2353-107">Get educationSubmission</span></span>

<span data-ttu-id="c2353-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2353-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2353-109">Recupere um envio específico.</span><span class="sxs-lookup"><span data-stu-id="c2353-109">Retrieve a particular submission.</span></span>

<span data-ttu-id="c2353-110">Um objeto de envio representa o trabalho de um aluno para uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="c2353-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="c2353-111">Os recursos associados ao envio representam esse trabalho.</span><span class="sxs-lookup"><span data-stu-id="c2353-111">Resources associated with the submission represent this work.</span></span> 

<span data-ttu-id="c2353-112">Somente o **aluno assignedTo** pode ver e modificar o envio.</span><span class="sxs-lookup"><span data-stu-id="c2353-112">Only the **assignedTo** student can see and modify the submission.</span></span> <span data-ttu-id="c2353-113">Um professor ou aplicativo com permissões de aplicativo tem acesso total a todos os envios.</span><span class="sxs-lookup"><span data-stu-id="c2353-113">A teacher or application with application permissions has full access to all submissions.</span></span>

<span data-ttu-id="c2353-114">As notas e os comentários de um professor fazem parte do [educationOutcome](../resources/educationoutcome.md) associado a esse objeto.</span><span class="sxs-lookup"><span data-stu-id="c2353-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="c2353-115">Somente professores ou aplicativos com permissões de aplicativo podem adicionar ou alterar notas e comentários.</span><span class="sxs-lookup"><span data-stu-id="c2353-115">Only teachers or applications with application permissions can add or change grades and feedback.</span></span> <span data-ttu-id="c2353-116">Os alunos não verão a nota ou os comentários até que a atribuição seja lançada.</span><span class="sxs-lookup"><span data-stu-id="c2353-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2353-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2353-117">Permissions</span></span>
<span data-ttu-id="c2353-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2353-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2353-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2353-120">Permission type</span></span>      | <span data-ttu-id="c2353-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2353-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2353-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2353-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="c2353-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2353-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="c2353-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2353-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c2353-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2353-125">Not supported.</span></span>  |
|<span data-ttu-id="c2353-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2353-126">Application</span></span> | <span data-ttu-id="c2353-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2353-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c2353-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2353-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2353-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2353-129">Optional query parameters</span></span>
<span data-ttu-id="c2353-130">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2353-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2353-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2353-131">Request headers</span></span>
| <span data-ttu-id="c2353-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2353-132">Header</span></span>       | <span data-ttu-id="c2353-133">Valor</span><span class="sxs-lookup"><span data-stu-id="c2353-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2353-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2353-134">Authorization</span></span>  | <span data-ttu-id="c2353-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2353-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2353-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2353-137">Request body</span></span>
<span data-ttu-id="c2353-138">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="c2353-138">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2353-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2353-139">Response</span></span>
<span data-ttu-id="c2353-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2353-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2353-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2353-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2353-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2353-142">Request</span></span>
<span data-ttu-id="c2353-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2353-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2353-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2353-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/11010/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/33223
```

### <a name="response"></a><span data-ttu-id="c2353-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2353-145">Response</span></span>
<span data-ttu-id="c2353-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2353-146">The following is an example of the response.</span></span> 

><span data-ttu-id="c2353-147">**Observações:** O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="c2353-147">**Notes:** The response object shown here might be shortened for readability.</span></span> 
>
><span data-ttu-id="c2353-148">Se [setUpResourcesFolder](educationsubmission-setupResourcesFolder.md) ainda não tiver sido chamado neste [recurso educationSubmission,](../resources/educationsubmission.md) a propriedade **resourcesFolderUrl** será `null` .</span><span class="sxs-lookup"><span data-stu-id="c2353-148">If [setUpResourcesFolder](educationsubmission-setupResourcesFolder.md) has not been called on this [educationSubmission](../resources/educationsubmission.md) resource yet, the **resourcesFolderUrl** property is `null`.</span></span>

<!-- {
  "blockType": "response",
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
