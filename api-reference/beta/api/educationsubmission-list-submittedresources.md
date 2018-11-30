---
title: Lista submittedResources
description: Lista os recursos que foram enviados para classificação oficialmente. O aluno proprietária o envio não pode alterar a lista enviada sem reenviar a atribuição. Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se este recurso foi copiado da atribuição.
ms.openlocfilehash: dba648d8a73ad2f2f91da7d7414214a62580cc99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038099"
---
# <a name="list-submittedresources"></a><span data-ttu-id="81a2e-105">Lista submittedResources</span><span class="sxs-lookup"><span data-stu-id="81a2e-105">List submittedResources</span></span>

> <span data-ttu-id="81a2e-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="81a2e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81a2e-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="81a2e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81a2e-108">Lista os recursos que foram enviados para classificação oficialmente.</span><span class="sxs-lookup"><span data-stu-id="81a2e-108">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="81a2e-109">O aluno proprietária o envio não pode alterar a lista enviada sem reenviar a atribuição.</span><span class="sxs-lookup"><span data-stu-id="81a2e-109">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="81a2e-110">Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se este recurso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="81a2e-110">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="81a2e-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="81a2e-111">Permissions</span></span>
<span data-ttu-id="81a2e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81a2e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a2e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81a2e-114">Permission type</span></span>      | <span data-ttu-id="81a2e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81a2e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81a2e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81a2e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="81a2e-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81a2e-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="81a2e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81a2e-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="81a2e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a2e-119">Not supported.</span></span>  |
|<span data-ttu-id="81a2e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81a2e-120">Application</span></span> | <span data-ttu-id="81a2e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a2e-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="81a2e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81a2e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81a2e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81a2e-123">Optional query parameters</span></span>
<span data-ttu-id="81a2e-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81a2e-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81a2e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81a2e-125">Request headers</span></span>
| <span data-ttu-id="81a2e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81a2e-126">Header</span></span>       | <span data-ttu-id="81a2e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="81a2e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81a2e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="81a2e-128">Authorization</span></span>  | <span data-ttu-id="81a2e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a2e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81a2e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81a2e-131">Request body</span></span>
<span data-ttu-id="81a2e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81a2e-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="81a2e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a2e-133">Response</span></span>
<span data-ttu-id="81a2e-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81a2e-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81a2e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81a2e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81a2e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81a2e-136">Request</span></span>
<span data-ttu-id="81a2e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81a2e-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="81a2e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a2e-138">Response</span></span>
<span data-ttu-id="81a2e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81a2e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="81a2e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81a2e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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