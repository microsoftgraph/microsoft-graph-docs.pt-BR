---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d833a566f6406a6ed1132053ad5ecbe83e6058c9
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061641"
---
# <a name="list-categories"></a><span data-ttu-id="b28cb-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="b28cb-103">List categories</span></span>

<span data-ttu-id="b28cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b28cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b28cb-105">Listar todas as categorias associadas a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="b28cb-105">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="b28cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b28cb-106">Permissions</span></span>
<span data-ttu-id="b28cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b28cb-109">Permission type</span></span>      | <span data-ttu-id="b28cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b28cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b28cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b28cb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b28cb-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b28cb-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b28cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b28cb-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b28cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28cb-114">Not supported.</span></span>  |
|<span data-ttu-id="b28cb-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="b28cb-115">Application\*</span></span> | <span data-ttu-id="b28cb-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b28cb-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="b28cb-117">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="b28cb-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="b28cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b28cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b28cb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b28cb-119">Optional query parameters</span></span>
<span data-ttu-id="b28cb-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b28cb-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b28cb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b28cb-121">Request headers</span></span>
| <span data-ttu-id="b28cb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b28cb-122">Header</span></span>       | <span data-ttu-id="b28cb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b28cb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b28cb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b28cb-124">Authorization</span></span>  | <span data-ttu-id="b28cb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b28cb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b28cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b28cb-127">Request body</span></span>
<span data-ttu-id="b28cb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b28cb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b28cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28cb-129">Response</span></span>
<span data-ttu-id="b28cb-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b28cb-130">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b28cb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b28cb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b28cb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b28cb-132">Request</span></span>
<span data-ttu-id="b28cb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b28cb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="b28cb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28cb-134">Response</span></span>
<span data-ttu-id="b28cb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b28cb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b28cb-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b28cb-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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