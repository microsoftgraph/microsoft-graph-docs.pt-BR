---
title: Criar educationCategory
description: Cria uma nova categoria.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6a2c92740db75350b5c1cefcd35c2b50723b55c
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911365"
---
# <a name="create-educationcategory"></a><span data-ttu-id="c7e7a-103">Criar educationCategory</span><span class="sxs-lookup"><span data-stu-id="c7e7a-103">Create educationCategory</span></span>

<span data-ttu-id="c7e7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7e7a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7e7a-105">Cria uma nova [educationCategory](../resources/educationcategory.md) em uma [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="c7e7a-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7e7a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7e7a-106">Permissions</span></span>
<span data-ttu-id="c7e7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7e7a-109">Permission type</span></span>      | <span data-ttu-id="c7e7a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7e7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7e7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7e7a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c7e7a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e7a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c7e7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7e7a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c7e7a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-114">Not supported.</span></span>  |
|<span data-ttu-id="c7e7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7e7a-115">Application</span></span> | <span data-ttu-id="c7e7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c7e7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7e7a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories/$entity
```
## <a name="request-headers"></a><span data-ttu-id="c7e7a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e7a-118">Request headers</span></span>
| <span data-ttu-id="c7e7a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7e7a-119">Header</span></span>       | <span data-ttu-id="c7e7a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c7e7a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7e7a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7e7a-121">Authorization</span></span>  | <span data-ttu-id="c7e7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7e7a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7e7a-124">Content-Type</span></span>  | <span data-ttu-id="c7e7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e7a-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7e7a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e7a-126">Request body</span></span>
<span data-ttu-id="c7e7a-127">No corpo da solicitação, fornece uma representação JSON de um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c7e7a-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c7e7a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e7a-128">Response</span></span>
<span data-ttu-id="c7e7a-129">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e7a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7e7a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7e7a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e7a-131">Request</span></span>
<span data-ttu-id="c7e7a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["60eaa744-aa87-4276-b985-1633683119f8"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/60eaa744-aa87-4276-b985-1633683119f8/assignmentCategories/$entity
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="c7e7a-133">No corpo da solicitação, fornece uma representação JSON de um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c7e7a-133">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="c7e7a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e7a-134">Response</span></span>
<span data-ttu-id="c7e7a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="c7e7a-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c7e7a-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 120

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('60eaa744-aa87-4276-b985-1633683119f8')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


