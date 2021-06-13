---
title: Listar recursos de envio
description: Listar os recursos associados a um envio.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 174f9fa606ab9f4a4bdc85fb60dd1e4f75d7ae39
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911792"
---
# <a name="list-submission-resources"></a><span data-ttu-id="7c8c3-103">Listar recursos de envio</span><span class="sxs-lookup"><span data-stu-id="7c8c3-103">List submission resources</span></span>

<span data-ttu-id="7c8c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c8c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c8c3-105">Listar os recursos associados a um envio.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-105">List the resources associated with a submission.</span></span> 

<span data-ttu-id="7c8c3-106">O **objeto submissionResource** é um wrapper em torno do objeto de recurso real em que o aluno está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="7c8c3-107">O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo de atribuição.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="7c8c3-108">Esses recursos são a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="7c8c3-109">Os **submittedResources** são os recursos que foram oficialmente enviados para serem gradeados.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c8c3-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c8c3-110">Permissions</span></span>

<span data-ttu-id="7c8c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c8c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c8c3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c8c3-113">Permission type</span></span>                        | <span data-ttu-id="7c8c3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c8c3-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7c8c3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c8c3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c8c3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c8c3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7c8c3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c8c3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c8c3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="7c8c3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c8c3-119">Application</span></span>                            | <span data-ttu-id="7c8c3-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c8c3-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c8c3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c8c3-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c8c3-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c8c3-122">Optional query parameters</span></span>

<span data-ttu-id="7c8c3-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c8c3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8c3-124">Request headers</span></span>

| <span data-ttu-id="7c8c3-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c8c3-125">Header</span></span>        | <span data-ttu-id="7c8c3-126">Valor</span><span class="sxs-lookup"><span data-stu-id="7c8c3-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7c8c3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c8c3-127">Authorization</span></span> | <span data-ttu-id="7c8c3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c8c3-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8c3-130">Request body</span></span>

<span data-ttu-id="7c8c3-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c8c3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8c3-132">Response</span></span>

<span data-ttu-id="7c8c3-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c8c3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c8c3-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c8c3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8c3-135">Request</span></span>

<span data-ttu-id="7c8c3-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7c8c3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c8c3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```
# <a name="c"></a>[<span data-ttu-id="7c8c3-138">C#</span><span class="sxs-lookup"><span data-stu-id="7c8c3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c8c3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c8c3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c8c3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c8c3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c8c3-141">Java</span><span class="sxs-lookup"><span data-stu-id="7c8c3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c8c3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8c3-142">Response</span></span>

<span data-ttu-id="7c8c3-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-143">The following is an example of the response.</span></span> 

><span data-ttu-id="7c8c3-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7c8c3-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
