---
title: Listar submittedResources
description: Liste os recursos que foram oficialmente enviados para a gradação. O aluno que possui o envio não pode alterar a lista enviada sem reenviar a atribuição. Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 371302640df794465764755492088ec2015278ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955114"
---
# <a name="list-submittedresources"></a><span data-ttu-id="368e3-105">Listar submittedResources</span><span class="sxs-lookup"><span data-stu-id="368e3-105">List submittedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="368e3-106">Liste os recursos que foram oficialmente enviados para a gradação.</span><span class="sxs-lookup"><span data-stu-id="368e3-106">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="368e3-107">O aluno que possui o envio não pode alterar a lista enviada sem reenviar a atribuição.</span><span class="sxs-lookup"><span data-stu-id="368e3-107">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="368e3-108">Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="368e3-108">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="368e3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="368e3-109">Permissions</span></span>
<span data-ttu-id="368e3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="368e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="368e3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="368e3-112">Permission type</span></span>      | <span data-ttu-id="368e3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="368e3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="368e3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="368e3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="368e3-115">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="368e3-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="368e3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="368e3-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="368e3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="368e3-117">Not supported.</span></span>  |
|<span data-ttu-id="368e3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="368e3-118">Application</span></span> | <span data-ttu-id="368e3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="368e3-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="368e3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="368e3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="368e3-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="368e3-121">Optional query parameters</span></span>
<span data-ttu-id="368e3-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="368e3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="368e3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="368e3-123">Request headers</span></span>
| <span data-ttu-id="368e3-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="368e3-124">Header</span></span>       | <span data-ttu-id="368e3-125">Valor</span><span class="sxs-lookup"><span data-stu-id="368e3-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="368e3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="368e3-126">Authorization</span></span>  | <span data-ttu-id="368e3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="368e3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="368e3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="368e3-129">Request body</span></span>
<span data-ttu-id="368e3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="368e3-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="368e3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="368e3-131">Response</span></span>
<span data-ttu-id="368e3-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="368e3-132">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="368e3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="368e3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="368e3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="368e3-134">Request</span></span>
<span data-ttu-id="368e3-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="368e3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="368e3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="368e3-136">Response</span></span>
<span data-ttu-id="368e3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="368e3-137">The following is an example of the response.</span></span> 

><span data-ttu-id="368e3-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="368e3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource",
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
        "link": "https://www.microsoft.com
        },
        "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource" 
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
