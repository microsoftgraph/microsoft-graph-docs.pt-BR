---
title: Listar submittedResources
description: Listar os recursos que foram enviados oficialmente para classificação. O aluno proprietário do envio não pode alterar a lista enviada sem reabrir a atribuição. Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 78e840e8517cb90881432189e4a057c4500e2a9c
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961125"
---
# <a name="list-submittedresources"></a><span data-ttu-id="ef2e2-105">Listar submittedResources</span><span class="sxs-lookup"><span data-stu-id="ef2e2-105">List submittedResources</span></span>

<span data-ttu-id="ef2e2-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef2e2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef2e2-107">Listar os recursos que foram enviados oficialmente para classificação.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-107">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="ef2e2-108">O aluno proprietário do envio não pode alterar a lista enviada sem reabrir a atribuição.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-108">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="ef2e2-109">Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-109">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef2e2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef2e2-110">Permissions</span></span>
<span data-ttu-id="ef2e2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef2e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef2e2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef2e2-113">Permission type</span></span>      | <span data-ttu-id="ef2e2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef2e2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef2e2-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef2e2-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ef2e2-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef2e2-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ef2e2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef2e2-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ef2e2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-118">Not supported.</span></span>  |
|<span data-ttu-id="ef2e2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef2e2-119">Application</span></span> | <span data-ttu-id="ef2e2-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef2e2-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ef2e2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef2e2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef2e2-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ef2e2-122">Optional query parameters</span></span>
<span data-ttu-id="ef2e2-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef2e2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef2e2-124">Request headers</span></span>
| <span data-ttu-id="ef2e2-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef2e2-125">Header</span></span>       | <span data-ttu-id="ef2e2-126">Valor</span><span class="sxs-lookup"><span data-stu-id="ef2e2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ef2e2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef2e2-127">Authorization</span></span>  | <span data-ttu-id="ef2e2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ef2e2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef2e2-130">Request body</span></span>
<span data-ttu-id="ef2e2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ef2e2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef2e2-132">Response</span></span>
<span data-ttu-id="ef2e2-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef2e2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef2e2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef2e2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef2e2-135">Request</span></span>
<span data-ttu-id="ef2e2-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="ef2e2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef2e2-137">Response</span></span>
<span data-ttu-id="ef2e2-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ef2e2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef2e2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
          "link": "https://www.microsoft.com"
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
