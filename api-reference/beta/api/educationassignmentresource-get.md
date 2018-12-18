---
title: Obter educationAssignmentResource
description: 'Obtenha as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
ms.openlocfilehash: 25c448f3247631c9129a837bd00842588bf152d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358811"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="e8db5-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e8db5-103">Get educationAssignmentResource</span></span>

> <span data-ttu-id="e8db5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8db5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8db5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8db5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8db5-106">Obtenha as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="e8db5-106">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="e8db5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8db5-107">Permissions</span></span>
<span data-ttu-id="e8db5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8db5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8db5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8db5-110">Permission type</span></span>      | <span data-ttu-id="e8db5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8db5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8db5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8db5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8db5-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8db5-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="e8db5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8db5-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8db5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8db5-115">Not supported.</span></span>  |
|<span data-ttu-id="e8db5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8db5-116">Application</span></span> |  <span data-ttu-id="e8db5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8db5-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e8db5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8db5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8db5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8db5-119">Optional query parameters</span></span>
<span data-ttu-id="e8db5-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8db5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8db5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8db5-121">Request headers</span></span>
| <span data-ttu-id="e8db5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8db5-122">Header</span></span>       | <span data-ttu-id="e8db5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e8db5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8db5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8db5-124">Authorization</span></span>  | <span data-ttu-id="e8db5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8db5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8db5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8db5-127">Request body</span></span>
<span data-ttu-id="e8db5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8db5-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e8db5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8db5-129">Response</span></span>
<span data-ttu-id="e8db5-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8db5-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8db5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8db5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8db5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8db5-132">Request</span></span>
<span data-ttu-id="e8db5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8db5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="e8db5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8db5-134">Response</span></span>
<span data-ttu-id="e8db5-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8db5-135">The following is an example of the response.</span></span> 

><span data-ttu-id="e8db5-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8db5-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8db5-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8db5-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->