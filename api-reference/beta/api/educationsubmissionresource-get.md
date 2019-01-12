---
title: Obter educationSubmissionResource
description: Recupera as propriedades de um recurso específico associado com o envio. Este recurso é na lista de recursos 'trabalho' e deve ser considerado de trabalho em andamento por um estudante. Este recurso é empacotado com um ponteiro possível de volta para o recurso de atribuição, se ele tiver sido copiado a atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47dd803e4a8503017d68f00c0e95c78ad271c870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940348"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="2ca70-105">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="2ca70-105">Get educationSubmissionResource</span></span>

> <span data-ttu-id="2ca70-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2ca70-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ca70-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2ca70-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ca70-108">Recupera as propriedades de um recurso específico associado com o envio.</span><span class="sxs-lookup"><span data-stu-id="2ca70-108">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="2ca70-109">Este recurso é na lista de recursos "trabalho" e deve ser considerado de trabalho em andamento por um estudante.</span><span class="sxs-lookup"><span data-stu-id="2ca70-109">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="2ca70-110">Este recurso é empacotado com um ponteiro possível de volta para o recurso de atribuição, se ele tiver sido copiado a atribuição.</span><span class="sxs-lookup"><span data-stu-id="2ca70-110">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ca70-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="2ca70-111">Permissions</span></span>
<span data-ttu-id="2ca70-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ca70-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca70-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ca70-114">Permission type</span></span>      | <span data-ttu-id="2ca70-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ca70-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ca70-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ca70-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="2ca70-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ca70-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2ca70-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ca70-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2ca70-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ca70-119">Not supported.</span></span>  |
|<span data-ttu-id="2ca70-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ca70-120">Application</span></span> | <span data-ttu-id="2ca70-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ca70-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2ca70-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ca70-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2ca70-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ca70-123">Optional query parameters</span></span>
<span data-ttu-id="2ca70-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca70-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ca70-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca70-125">Request headers</span></span>
| <span data-ttu-id="2ca70-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ca70-126">Header</span></span>       | <span data-ttu-id="2ca70-127">Valor</span><span class="sxs-lookup"><span data-stu-id="2ca70-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ca70-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ca70-128">Authorization</span></span>  | <span data-ttu-id="2ca70-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ca70-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ca70-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca70-131">Request body</span></span>
<span data-ttu-id="2ca70-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ca70-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2ca70-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca70-133">Response</span></span>
<span data-ttu-id="2ca70-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca70-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ca70-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ca70-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ca70-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca70-136">Request</span></span>
<span data-ttu-id="2ca70-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ca70-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="2ca70-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca70-138">Response</span></span>
<span data-ttu-id="2ca70-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca70-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2ca70-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ca70-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
