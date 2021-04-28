---
title: Listar submittedResources
description: Listar os recursos que foram enviados oficialmente para classificação. O aluno proprietário do envio não pode alterar a lista enviada sem reabrir a atribuição. Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 861ee3371517d95e89c9077d6e139202d370a917
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061837"
---
# <a name="list-submittedresources"></a><span data-ttu-id="3c6ce-105">Listar submittedResources</span><span class="sxs-lookup"><span data-stu-id="3c6ce-105">List submittedResources</span></span>

<span data-ttu-id="3c6ce-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c6ce-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c6ce-107">Listar os recursos que foram enviados oficialmente para classificação.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-107">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="3c6ce-108">O aluno proprietário do envio não pode alterar a lista enviada sem reabrir a atribuição.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-108">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="3c6ce-109">Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-109">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c6ce-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c6ce-110">Permissions</span></span>
<span data-ttu-id="3c6ce-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c6ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c6ce-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c6ce-113">Permission type</span></span>      | <span data-ttu-id="3c6ce-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c6ce-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c6ce-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c6ce-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="3c6ce-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c6ce-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3c6ce-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c6ce-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3c6ce-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-118">Not supported.</span></span>  |
|<span data-ttu-id="3c6ce-119">Application\*</span><span class="sxs-lookup"><span data-stu-id="3c6ce-119">Application\*</span></span> | <span data-ttu-id="3c6ce-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c6ce-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="3c6ce-121">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c6ce-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c6ce-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c6ce-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c6ce-123">Optional query parameters</span></span>
<span data-ttu-id="3c6ce-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c6ce-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c6ce-125">Request headers</span></span>
| <span data-ttu-id="3c6ce-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c6ce-126">Header</span></span>       | <span data-ttu-id="3c6ce-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3c6ce-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c6ce-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c6ce-128">Authorization</span></span>  | <span data-ttu-id="3c6ce-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c6ce-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c6ce-131">Request body</span></span>
<span data-ttu-id="3c6ce-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3c6ce-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c6ce-133">Response</span></span>
<span data-ttu-id="3c6ce-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c6ce-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c6ce-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c6ce-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c6ce-136">Request</span></span>
<span data-ttu-id="3c6ce-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="3c6ce-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c6ce-138">Response</span></span>
<span data-ttu-id="3c6ce-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-139">The following is an example of the response.</span></span> 

><span data-ttu-id="3c6ce-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c6ce-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
