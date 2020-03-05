---
title: Listar recursos
description: Listar os recursos associados a esse envio. O objeto **submissionResource** é um invólucro em torno do objeto de recurso real em que o aluno está trabalhando. O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo assign. Esses recursos são a cópia de trabalho da atribuição. Os **submittedResources** são os recursos que foram enviados oficialmente para serem comparados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 61c887d507e52da0883b127b3c6123c073de04e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425139"
---
# <a name="list-resources"></a><span data-ttu-id="83d9e-107">Listar recursos</span><span class="sxs-lookup"><span data-stu-id="83d9e-107">List resources</span></span>

<span data-ttu-id="83d9e-108">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="83d9e-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83d9e-109">Listar os recursos associados a esse envio.</span><span class="sxs-lookup"><span data-stu-id="83d9e-109">List the resources associated with this submission.</span></span> <span data-ttu-id="83d9e-110">O objeto **submissionResource** é um invólucro em torno do objeto de recurso real em que o aluno está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="83d9e-110">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="83d9e-111">O wrapper também inclui um ponteiro para os recursos na atribuição se ele foi copiado da atribuição durante o processo assign.</span><span class="sxs-lookup"><span data-stu-id="83d9e-111">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="83d9e-112">Esses recursos são a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="83d9e-112">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="83d9e-113">Os **submittedResources** são os recursos que foram enviados oficialmente para serem comparados.</span><span class="sxs-lookup"><span data-stu-id="83d9e-113">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="83d9e-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="83d9e-114">Permissions</span></span>

<span data-ttu-id="83d9e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d9e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83d9e-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83d9e-117">Permission type</span></span>                        | <span data-ttu-id="83d9e-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83d9e-118">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="83d9e-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83d9e-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="83d9e-120">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83d9e-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="83d9e-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83d9e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83d9e-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d9e-122">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="83d9e-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83d9e-123">Application</span></span>                            | <span data-ttu-id="83d9e-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d9e-124">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="83d9e-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83d9e-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83d9e-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83d9e-126">Optional query parameters</span></span>

<span data-ttu-id="83d9e-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83d9e-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83d9e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83d9e-128">Request headers</span></span>

| <span data-ttu-id="83d9e-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83d9e-129">Header</span></span>        | <span data-ttu-id="83d9e-130">Valor</span><span class="sxs-lookup"><span data-stu-id="83d9e-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="83d9e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="83d9e-131">Authorization</span></span> | <span data-ttu-id="83d9e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d9e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83d9e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83d9e-134">Request body</span></span>

<span data-ttu-id="83d9e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83d9e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83d9e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d9e-136">Response</span></span>

<span data-ttu-id="83d9e-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83d9e-137">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83d9e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83d9e-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83d9e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83d9e-139">Request</span></span>

<span data-ttu-id="83d9e-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83d9e-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

##### <a name="response"></a><span data-ttu-id="83d9e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d9e-141">Response</span></span>

<span data-ttu-id="83d9e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83d9e-142">The following is an example of the response.</span></span> 

><span data-ttu-id="83d9e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83d9e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
