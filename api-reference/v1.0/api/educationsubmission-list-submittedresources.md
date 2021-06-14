---
title: Listar submittedResources
description: Listar os recursos que foram enviados oficialmente para classificação.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7aaaaf7d4ec003a4f7d6e04082422a08dec4681d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911380"
---
# <a name="list-submittedresources"></a><span data-ttu-id="d603e-103">Listar submittedResources</span><span class="sxs-lookup"><span data-stu-id="d603e-103">List submittedResources</span></span>

<span data-ttu-id="d603e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d603e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d603e-105">Listar os recursos que foram enviados oficialmente para classificação.</span><span class="sxs-lookup"><span data-stu-id="d603e-105">List the resources that have officially been submitted for grading.</span></span> 

<span data-ttu-id="d603e-106">O aluno proprietário do envio não pode alterar a lista enviada sem reabrir a atribuição.</span><span class="sxs-lookup"><span data-stu-id="d603e-106">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="d603e-107">Este é um wrapper em torno do recurso real e pode conter um ponteiro de volta para o recurso de atribuição real se esse recurso foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d603e-107">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d603e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d603e-108">Permissions</span></span>
<span data-ttu-id="d603e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d603e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d603e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d603e-111">Permission type</span></span>      | <span data-ttu-id="d603e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d603e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d603e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d603e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="d603e-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d603e-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d603e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d603e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d603e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d603e-116">Not supported.</span></span>  |
|<span data-ttu-id="d603e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d603e-117">Application</span></span> | <span data-ttu-id="d603e-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d603e-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d603e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d603e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d603e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d603e-120">Optional query parameters</span></span>
<span data-ttu-id="d603e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d603e-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d603e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d603e-122">Request headers</span></span>
| <span data-ttu-id="d603e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d603e-123">Header</span></span>       | <span data-ttu-id="d603e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d603e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d603e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d603e-125">Authorization</span></span>  | <span data-ttu-id="d603e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d603e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d603e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d603e-128">Request body</span></span>
<span data-ttu-id="d603e-129">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="d603e-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d603e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d603e-130">Response</span></span>
<span data-ttu-id="d603e-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d603e-131">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d603e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d603e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="d603e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d603e-133">Request</span></span>
<span data-ttu-id="d603e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d603e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_submittedresources"
}-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submittedResources
```
### <a name="response"></a><span data-ttu-id="d603e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d603e-135">Response</span></span>
<span data-ttu-id="d603e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d603e-136">The following is an example of the response.</span></span> 

><span data-ttu-id="d603e-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d603e-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
        "assignmentResourceUrl": null,
        "id": "0f7dd681-f1b6-4f78-b8fb-a579fc4a36ae",
        "resource": {
            "@odata.type": "#microsoft.graph.educationLinkResource",
            "displayName": "ABC",
            "createdDateTime": "2021-03-11T20:47:53.0823323Z",
            "lastModifiedDateTime": "2021-03-11T20:47:53.0823323Z",
            "link": "https://www.bing.com/",
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
                    "displayName": null
                }
            }
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
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
