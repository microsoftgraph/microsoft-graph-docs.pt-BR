---
title: Obter educationSubmission
description: 'Recupere um envio específico. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao que o envio é atribuído pode ver e modificar o envio. Um professor ou aplicativo com permissões de aplicativo tem acesso total a todos os envios. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 46b04c06497075d9abdb8e09533c46f752fb3e92
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118984"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="c5866-107">Obter educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c5866-107">Get educationSubmission</span></span>

<span data-ttu-id="c5866-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5866-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5866-109">Recupere um envio específico.</span><span class="sxs-lookup"><span data-stu-id="c5866-109">Retrieve a particular submission.</span></span> <span data-ttu-id="c5866-110">Um objeto de envio representa o trabalho de um aluno para uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="c5866-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="c5866-111">Os recursos associados ao envio representam esse trabalho.</span><span class="sxs-lookup"><span data-stu-id="c5866-111">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="c5866-112">Somente o aluno ao que o envio é atribuído pode ver e modificar o envio.</span><span class="sxs-lookup"><span data-stu-id="c5866-112">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="c5866-113">Um professor ou aplicativo com permissões de aplicativo tem acesso total a todos os envios.</span><span class="sxs-lookup"><span data-stu-id="c5866-113">A teacher or application with application permissions has full access to all submissions.</span></span>

<span data-ttu-id="c5866-114">As notas e os comentários de um professor fazem parte do [educationOutcome](../resources/educationoutcome.md) associado a esse objeto.</span><span class="sxs-lookup"><span data-stu-id="c5866-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="c5866-115">Somente professores ou aplicativos com permissões de aplicativo podem adicionar ou alterar notas e comentários.</span><span class="sxs-lookup"><span data-stu-id="c5866-115">Only teachers or applications with application permissions can add or change grades and feedback.</span></span> <span data-ttu-id="c5866-116">Os alunos não verão a nota ou os comentários até que a atribuição seja lançada.</span><span class="sxs-lookup"><span data-stu-id="c5866-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5866-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5866-117">Permissions</span></span>
<span data-ttu-id="c5866-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5866-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5866-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5866-120">Permission type</span></span>      | <span data-ttu-id="c5866-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5866-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5866-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5866-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="c5866-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5866-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="c5866-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5866-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c5866-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5866-125">Not supported.</span></span>  |
|<span data-ttu-id="c5866-126">Application\*</span><span class="sxs-lookup"><span data-stu-id="c5866-126">Application\*</span></span> | <span data-ttu-id="c5866-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5866-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="c5866-128">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="c5866-128">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5866-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5866-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5866-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5866-130">Optional query parameters</span></span>
<span data-ttu-id="c5866-131">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5866-131">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5866-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5866-132">Request headers</span></span>
| <span data-ttu-id="c5866-133">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5866-133">Header</span></span>       | <span data-ttu-id="c5866-134">Valor</span><span class="sxs-lookup"><span data-stu-id="c5866-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5866-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5866-135">Authorization</span></span>  | <span data-ttu-id="c5866-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5866-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5866-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5866-138">Request body</span></span>
<span data-ttu-id="c5866-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5866-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c5866-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5866-140">Response</span></span>
<span data-ttu-id="c5866-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5866-141">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5866-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5866-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5866-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5866-143">Request</span></span>
<span data-ttu-id="c5866-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5866-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5866-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5866-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
# <a name="c"></a>[<span data-ttu-id="c5866-146">C#</span><span class="sxs-lookup"><span data-stu-id="c5866-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5866-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5866-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5866-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5866-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5866-149">Java</span><span class="sxs-lookup"><span data-stu-id="c5866-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5866-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5866-150">Response</span></span>
<span data-ttu-id="c5866-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5866-151">The following is an example of the response.</span></span> 

><span data-ttu-id="c5866-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5866-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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
