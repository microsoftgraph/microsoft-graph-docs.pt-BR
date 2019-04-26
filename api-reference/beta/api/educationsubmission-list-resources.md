---
title: Listar recursos
description: Listar os recursos associados a esse envio. O objeto **submissionResource** é um invólucro em torno do objeto de recurso real em que o aluno está trabalhando. O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo assign. Esses recursos são a cópia de trabalho da atribuição. Os **submittedResources** são os recursos que foram enviados oficialmente para serem comparados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8b1759e2dca969acb0db1a287099ef97e810e064
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322882"
---
# <a name="list-resources"></a><span data-ttu-id="e7ea2-107">Listar recursos</span><span class="sxs-lookup"><span data-stu-id="e7ea2-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7ea2-108">Listar os recursos associados a esse envio.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-108">List the resources associated with this submission.</span></span> <span data-ttu-id="e7ea2-109">O objeto **submissionResource** é um invólucro em torno do objeto de recurso real em que o aluno está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="e7ea2-110">O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo assign.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="e7ea2-111">Esses recursos são a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="e7ea2-112">Os **submittedResources** são os recursos que foram enviados oficialmente para serem comparados.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7ea2-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7ea2-113">Permissions</span></span>
<span data-ttu-id="e7ea2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7ea2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ea2-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7ea2-116">Permission type</span></span>      | <span data-ttu-id="e7ea2-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7ea2-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7ea2-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7ea2-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="e7ea2-119">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7ea2-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e7ea2-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7ea2-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7ea2-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-121">Not supported.</span></span>   |
|<span data-ttu-id="e7ea2-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7ea2-122">Application</span></span> | <span data-ttu-id="e7ea2-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e7ea2-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7ea2-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7ea2-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7ea2-125">Optional query parameters</span></span>
<span data-ttu-id="e7ea2-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7ea2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7ea2-127">Request headers</span></span>
| <span data-ttu-id="e7ea2-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7ea2-128">Header</span></span>       | <span data-ttu-id="e7ea2-129">Valor</span><span class="sxs-lookup"><span data-stu-id="e7ea2-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7ea2-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7ea2-130">Authorization</span></span>  | <span data-ttu-id="e7ea2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7ea2-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7ea2-133">Request body</span></span>
<span data-ttu-id="e7ea2-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e7ea2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7ea2-135">Response</span></span>
<span data-ttu-id="e7ea2-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7ea2-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7ea2-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7ea2-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7ea2-138">Request</span></span>
<span data-ttu-id="e7ea2-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="e7ea2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7ea2-140">Response</span></span>
<span data-ttu-id="e7ea2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-141">The following is an example of the response.</span></span> 

><span data-ttu-id="e7ea2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7ea2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
