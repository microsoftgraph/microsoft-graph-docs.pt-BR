---
title: Criar educationCategory
description: Cria uma nova categoria.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: eb169310f77e2f4f13a06dbb9871db07dc392101
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324638"
---
# <a name="create-educationcategory"></a><span data-ttu-id="d5035-103">Criar educationCategory</span><span class="sxs-lookup"><span data-stu-id="d5035-103">Create educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5035-104">Cria um novo [educationCategory](../resources/educationcategory.md) em um [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="d5035-104">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5035-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5035-105">Permissions</span></span>
<span data-ttu-id="d5035-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5035-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5035-108">Permission type</span></span>      | <span data-ttu-id="d5035-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5035-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5035-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5035-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d5035-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5035-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d5035-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5035-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d5035-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5035-113">Not supported.</span></span>  |
|<span data-ttu-id="d5035-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5035-114">Application</span></span> | <span data-ttu-id="d5035-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5035-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d5035-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5035-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="d5035-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5035-117">Request headers</span></span>
| <span data-ttu-id="d5035-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5035-118">Header</span></span>       | <span data-ttu-id="d5035-119">Valor</span><span class="sxs-lookup"><span data-stu-id="d5035-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d5035-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5035-120">Authorization</span></span>  | <span data-ttu-id="d5035-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5035-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d5035-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5035-123">Content-Type</span></span>  | <span data-ttu-id="d5035-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d5035-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5035-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5035-125">Request body</span></span>
<span data-ttu-id="d5035-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationCategory](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d5035-126">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d5035-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5035-127">Response</span></span>
<span data-ttu-id="d5035-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5035-128">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5035-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5035-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5035-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5035-130">Request</span></span>
<span data-ttu-id="d5035-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5035-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="d5035-132">No corpo da solicitação, forneça uma representação JSON de um objeto [educationCategory](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d5035-132">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d5035-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5035-133">Response</span></span>
<span data-ttu-id="d5035-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5035-134">The following is an example of the response.</span></span> 

><span data-ttu-id="d5035-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5035-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
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
