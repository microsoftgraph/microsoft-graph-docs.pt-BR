---
title: Remover educationClass
description: Exclua uma classe de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0b7ac85788c99cf5ba9773a5caced43e4f098386
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324845"
---
# <a name="remove-educationclass"></a><span data-ttu-id="d0fc3-103">Remover educationClass</span><span class="sxs-lookup"><span data-stu-id="d0fc3-103">Remove educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0fc3-104">Exclua uma classe de uma escola.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0fc3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0fc3-105">Permissions</span></span>
<span data-ttu-id="d0fc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0fc3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0fc3-108">Permission type</span></span>      | <span data-ttu-id="d0fc3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0fc3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d0fc3-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-111">Not supported.</span></span>  |
|<span data-ttu-id="d0fc3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0fc3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-113">Not supported.</span></span>  |
|<span data-ttu-id="d0fc3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0fc3-114">Application</span></span> | <span data-ttu-id="d0fc3-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0fc3-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0fc3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0fc3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d0fc3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0fc3-117">Request headers</span></span>
| <span data-ttu-id="d0fc3-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0fc3-118">Header</span></span>       | <span data-ttu-id="d0fc3-119">Valor</span><span class="sxs-lookup"><span data-stu-id="d0fc3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0fc3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0fc3-120">Authorization</span></span>  | <span data-ttu-id="d0fc3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0fc3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0fc3-123">Request body</span></span>
<span data-ttu-id="d0fc3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d0fc3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0fc3-125">Response</span></span>
<span data-ttu-id="d0fc3-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0fc3-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0fc3-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0fc3-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0fc3-128">Request</span></span>
<span data-ttu-id="d0fc3-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="d0fc3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0fc3-130">Response</span></span>
<span data-ttu-id="d0fc3-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
