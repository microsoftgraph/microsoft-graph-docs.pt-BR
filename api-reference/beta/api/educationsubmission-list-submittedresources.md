---
title: Lista submittedResources
description: Lista os recursos que foram enviados para classificação oficialmente. O aluno proprietária o envio não pode alterar a lista enviada sem reenviar a atribuição. Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se este recurso foi copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: da036713e6683aaef6576145dfe32b3b6eeaf11e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824140"
---
# <a name="list-submittedresources"></a><span data-ttu-id="122fe-105">Lista submittedResources</span><span class="sxs-lookup"><span data-stu-id="122fe-105">List submittedResources</span></span>

> <span data-ttu-id="122fe-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="122fe-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="122fe-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="122fe-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="122fe-108">Lista os recursos que foram enviados para classificação oficialmente.</span><span class="sxs-lookup"><span data-stu-id="122fe-108">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="122fe-109">O aluno proprietária o envio não pode alterar a lista enviada sem reenviar a atribuição.</span><span class="sxs-lookup"><span data-stu-id="122fe-109">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="122fe-110">Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se este recurso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="122fe-110">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="122fe-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="122fe-111">Permissions</span></span>
<span data-ttu-id="122fe-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="122fe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="122fe-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="122fe-114">Permission type</span></span>      | <span data-ttu-id="122fe-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="122fe-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="122fe-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="122fe-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="122fe-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="122fe-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="122fe-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="122fe-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="122fe-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="122fe-119">Not supported.</span></span>  |
|<span data-ttu-id="122fe-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="122fe-120">Application</span></span> | <span data-ttu-id="122fe-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="122fe-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="122fe-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="122fe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="122fe-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="122fe-123">Optional query parameters</span></span>
<span data-ttu-id="122fe-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="122fe-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="122fe-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="122fe-125">Request headers</span></span>
| <span data-ttu-id="122fe-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="122fe-126">Header</span></span>       | <span data-ttu-id="122fe-127">Valor</span><span class="sxs-lookup"><span data-stu-id="122fe-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="122fe-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="122fe-128">Authorization</span></span>  | <span data-ttu-id="122fe-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="122fe-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="122fe-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="122fe-131">Request body</span></span>
<span data-ttu-id="122fe-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="122fe-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="122fe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="122fe-133">Response</span></span>
<span data-ttu-id="122fe-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="122fe-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="122fe-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="122fe-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="122fe-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="122fe-136">Request</span></span>
<span data-ttu-id="122fe-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="122fe-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="122fe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="122fe-138">Response</span></span>
<span data-ttu-id="122fe-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="122fe-139">The following is an example of the response.</span></span> 

><span data-ttu-id="122fe-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="122fe-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
