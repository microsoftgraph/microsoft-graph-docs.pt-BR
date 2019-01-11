---
title: Remover professor
description: Remova um professor de uma aula.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 444b97fb5fa25c7863b0607455752956dc6396f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836320"
---
# <a name="remove-teacher"></a><span data-ttu-id="34167-103">Remover professor</span><span class="sxs-lookup"><span data-stu-id="34167-103">Remove teacher</span></span>

<span data-ttu-id="34167-104">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="34167-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="34167-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34167-105">Permissions</span></span>
<span data-ttu-id="34167-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34167-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34167-108">Permission type</span></span>      | <span data-ttu-id="34167-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34167-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34167-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34167-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="34167-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34167-111">Not supported.</span></span>  |
|<span data-ttu-id="34167-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34167-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="34167-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34167-113">Not supported.</span></span>  |
|<span data-ttu-id="34167-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34167-114">Application</span></span> | <span data-ttu-id="34167-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34167-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="34167-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34167-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="34167-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34167-117">Request headers</span></span>
| <span data-ttu-id="34167-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34167-118">Header</span></span>       | <span data-ttu-id="34167-119">Valor</span><span class="sxs-lookup"><span data-stu-id="34167-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34167-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="34167-120">Authorization</span></span>  | <span data-ttu-id="34167-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34167-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34167-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34167-123">Request body</span></span>
<span data-ttu-id="34167-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34167-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="34167-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="34167-125">Response</span></span>
<span data-ttu-id="34167-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="34167-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="34167-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34167-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34167-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34167-128">Request</span></span>
<span data-ttu-id="34167-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34167-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="34167-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="34167-130">Response</span></span>
<span data-ttu-id="34167-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34167-131">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
