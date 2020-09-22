---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d2c093c674fe99659b648204f39d72b72aed9b33
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007792"
---
# <a name="list-categories"></a><span data-ttu-id="8e09e-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="8e09e-103">List categories</span></span>

<span data-ttu-id="8e09e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e09e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e09e-105">Listar todas as categorias associadas a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="8e09e-105">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e09e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e09e-106">Permissions</span></span>
<span data-ttu-id="8e09e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e09e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e09e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e09e-109">Permission type</span></span>      | <span data-ttu-id="8e09e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e09e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e09e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e09e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e09e-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e09e-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8e09e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e09e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e09e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e09e-114">Not supported.</span></span>  |
|<span data-ttu-id="8e09e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e09e-115">Application</span></span> | <span data-ttu-id="8e09e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e09e-116">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8e09e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e09e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e09e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e09e-118">Optional query parameters</span></span>
<span data-ttu-id="8e09e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e09e-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e09e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e09e-120">Request headers</span></span>
| <span data-ttu-id="8e09e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e09e-121">Header</span></span>       | <span data-ttu-id="8e09e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e09e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e09e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e09e-123">Authorization</span></span>  | <span data-ttu-id="8e09e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e09e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e09e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e09e-126">Request body</span></span>
<span data-ttu-id="8e09e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e09e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8e09e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e09e-128">Response</span></span>
<span data-ttu-id="8e09e-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e09e-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e09e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e09e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e09e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e09e-131">Request</span></span>
<span data-ttu-id="8e09e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e09e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="8e09e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e09e-133">Response</span></span>
<span data-ttu-id="8e09e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e09e-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8e09e-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8e09e-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e09e-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e09e-136">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


