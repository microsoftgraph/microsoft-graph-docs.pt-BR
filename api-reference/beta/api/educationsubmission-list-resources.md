---
title: Listar recursos
description: Listar os recursos associados a esse envio. O **objeto submissionResource** é um wrapper em torno do objeto de recurso real em que o aluno está trabalhando. O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo de atribuição. Esses recursos são a cópia de trabalho da atribuição. Os **submittedResources** são os recursos que foram oficialmente enviados para serem gradeados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6043486becec97976648f67f06a4051aa431b7ae
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961209"
---
# <a name="list-resources"></a><span data-ttu-id="c9e28-107">Listar recursos</span><span class="sxs-lookup"><span data-stu-id="c9e28-107">List resources</span></span>

<span data-ttu-id="c9e28-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9e28-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9e28-109">Listar os recursos associados a esse envio.</span><span class="sxs-lookup"><span data-stu-id="c9e28-109">List the resources associated with this submission.</span></span> <span data-ttu-id="c9e28-110">O **objeto submissionResource** é um wrapper em torno do objeto de recurso real em que o aluno está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="c9e28-110">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="c9e28-111">O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo de atribuição.</span><span class="sxs-lookup"><span data-stu-id="c9e28-111">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="c9e28-112">Esses recursos são a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c9e28-112">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="c9e28-113">Os **submittedResources** são os recursos que foram oficialmente enviados para serem gradeados.</span><span class="sxs-lookup"><span data-stu-id="c9e28-113">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9e28-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9e28-114">Permissions</span></span>

<span data-ttu-id="c9e28-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9e28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9e28-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9e28-117">Permission type</span></span>                        | <span data-ttu-id="c9e28-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9e28-118">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c9e28-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9e28-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9e28-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9e28-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c9e28-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9e28-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9e28-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9e28-122">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="c9e28-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9e28-123">Application</span></span>                            | <span data-ttu-id="c9e28-124">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9e28-124">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9e28-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9e28-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9e28-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9e28-126">Optional query parameters</span></span>

<span data-ttu-id="c9e28-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9e28-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9e28-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e28-128">Request headers</span></span>

| <span data-ttu-id="c9e28-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9e28-129">Header</span></span>        | <span data-ttu-id="c9e28-130">Valor</span><span class="sxs-lookup"><span data-stu-id="c9e28-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c9e28-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9e28-131">Authorization</span></span> | <span data-ttu-id="c9e28-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9e28-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9e28-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e28-134">Request body</span></span>

<span data-ttu-id="c9e28-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9e28-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e28-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9e28-136">Response</span></span>

<span data-ttu-id="c9e28-137">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9e28-137">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9e28-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9e28-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9e28-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e28-139">Request</span></span>

<span data-ttu-id="c9e28-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9e28-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c9e28-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9e28-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```
# <a name="c"></a>[<span data-ttu-id="c9e28-142">C#</span><span class="sxs-lookup"><span data-stu-id="c9e28-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9e28-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9e28-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9e28-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9e28-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9e28-145">Java</span><span class="sxs-lookup"><span data-stu-id="c9e28-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c9e28-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9e28-146">Response</span></span>

<span data-ttu-id="c9e28-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9e28-147">The following is an example of the response.</span></span> 

><span data-ttu-id="c9e28-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9e28-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
