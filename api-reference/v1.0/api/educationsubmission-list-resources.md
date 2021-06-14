---
title: Listar recursos de envio
description: Listar os recursos associados a um envio.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d291ac67988d3960c70df1f8183b0c8989ce008
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911389"
---
# <a name="list-submission-resources"></a><span data-ttu-id="739cd-103">Listar recursos de envio</span><span class="sxs-lookup"><span data-stu-id="739cd-103">List submission resources</span></span>

<span data-ttu-id="739cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="739cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="739cd-105">Listar os recursos associados a um [envio](../resources/educationsubmission.md).</span><span class="sxs-lookup"><span data-stu-id="739cd-105">List the resources associated with a [submission](../resources/educationsubmission.md).</span></span> 

<span data-ttu-id="739cd-106">O **objeto submissionResource** é um wrapper em torno do objeto de recurso real em que o aluno está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="739cd-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="739cd-107">O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo de atribuição.</span><span class="sxs-lookup"><span data-stu-id="739cd-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="739cd-108">Esses recursos são a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="739cd-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="739cd-109">Os **submittedResources** são os recursos que foram oficialmente enviados para serem gradeados.</span><span class="sxs-lookup"><span data-stu-id="739cd-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="739cd-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="739cd-110">Permissions</span></span>

<span data-ttu-id="739cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="739cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="739cd-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="739cd-113">Permission type</span></span>                        | <span data-ttu-id="739cd-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="739cd-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="739cd-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="739cd-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="739cd-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="739cd-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="739cd-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="739cd-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="739cd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="739cd-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="739cd-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="739cd-119">Application</span></span>                            | <span data-ttu-id="739cd-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="739cd-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="739cd-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="739cd-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="739cd-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="739cd-122">Optional query parameters</span></span>

<span data-ttu-id="739cd-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="739cd-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="739cd-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="739cd-124">Request headers</span></span>

| <span data-ttu-id="739cd-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="739cd-125">Header</span></span>        | <span data-ttu-id="739cd-126">Valor</span><span class="sxs-lookup"><span data-stu-id="739cd-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="739cd-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="739cd-127">Authorization</span></span> | <span data-ttu-id="739cd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="739cd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="739cd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="739cd-130">Request body</span></span>

<span data-ttu-id="739cd-131">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="739cd-131">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="739cd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="739cd-132">Response</span></span>

<span data-ttu-id="739cd-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="739cd-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="739cd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="739cd-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="739cd-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="739cd-135">Request</span></span>

<span data-ttu-id="739cd-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="739cd-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

### <a name="response"></a><span data-ttu-id="739cd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="739cd-137">Response</span></span>

<span data-ttu-id="739cd-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="739cd-138">The following is an example of the response.</span></span> 

><span data-ttu-id="739cd-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="739cd-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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
