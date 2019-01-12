---
title: Lista de recursos
description: Lista os recursos associados a esse envio. O objeto de **submissionResource** é que um wrapper ao redor do objeto de recurso real do aluno está funcionando no. O wrapper também inclui um ponteiro para os recursos na atribuição se isso foi copiado da atribuição durante o processo de atribuir. Esses recursos estão a cópia de trabalho da atribuição. O **submittedResources** são os recursos que foram enviados para ser graduadas oficialmente.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bff80bd7975171f277cb8e6e6ee08cfd250a67ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975357"
---
# <a name="list-resources"></a><span data-ttu-id="6090a-107">Lista de recursos</span><span class="sxs-lookup"><span data-stu-id="6090a-107">List resources</span></span>

> <span data-ttu-id="6090a-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6090a-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6090a-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6090a-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6090a-110">Lista os recursos associados a esse envio.</span><span class="sxs-lookup"><span data-stu-id="6090a-110">List the resources associated with this submission.</span></span> <span data-ttu-id="6090a-111">O objeto de **submissionResource** é que um wrapper ao redor do objeto de recurso real do aluno está funcionando no.</span><span class="sxs-lookup"><span data-stu-id="6090a-111">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="6090a-112">O wrapper também inclui um ponteiro para os recursos na atribuição se isso foi copiado da atribuição durante o processo de atribuir.</span><span class="sxs-lookup"><span data-stu-id="6090a-112">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="6090a-113">Esses recursos estão a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6090a-113">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="6090a-114">O **submittedResources** são os recursos que foram enviados para ser graduadas oficialmente.</span><span class="sxs-lookup"><span data-stu-id="6090a-114">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="6090a-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="6090a-115">Permissions</span></span>
<span data-ttu-id="6090a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6090a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6090a-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6090a-118">Permission type</span></span>      | <span data-ttu-id="6090a-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6090a-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6090a-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6090a-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="6090a-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6090a-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6090a-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6090a-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6090a-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6090a-123">Not supported.</span></span>   |
|<span data-ttu-id="6090a-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6090a-124">Application</span></span> | <span data-ttu-id="6090a-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6090a-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6090a-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6090a-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6090a-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6090a-127">Optional query parameters</span></span>
<span data-ttu-id="6090a-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6090a-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6090a-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6090a-129">Request headers</span></span>
| <span data-ttu-id="6090a-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6090a-130">Header</span></span>       | <span data-ttu-id="6090a-131">Valor</span><span class="sxs-lookup"><span data-stu-id="6090a-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6090a-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="6090a-132">Authorization</span></span>  | <span data-ttu-id="6090a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6090a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6090a-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6090a-135">Request body</span></span>
<span data-ttu-id="6090a-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6090a-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6090a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6090a-137">Response</span></span>
<span data-ttu-id="6090a-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6090a-138">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6090a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6090a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6090a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6090a-140">Request</span></span>
<span data-ttu-id="6090a-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6090a-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="6090a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6090a-142">Response</span></span>
<span data-ttu-id="6090a-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6090a-143">The following is an example of the response.</span></span> 

><span data-ttu-id="6090a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6090a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
