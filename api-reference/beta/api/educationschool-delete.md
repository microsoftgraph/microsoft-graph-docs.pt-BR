---
title: Excluir educationSchool
description: Exclua uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b3235096a3ceac2a6b1037bc27cd0b83afbd7bd2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457668"
---
# <a name="delete-educationschool"></a><span data-ttu-id="7879e-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="7879e-103">Delete educationSchool</span></span>

<span data-ttu-id="7879e-104">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="7879e-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="7879e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7879e-105">Permissions</span></span>
<span data-ttu-id="7879e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7879e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7879e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7879e-108">Permission type</span></span>      | <span data-ttu-id="7879e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7879e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7879e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7879e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7879e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7879e-111">Not supported.</span></span>  |
|<span data-ttu-id="7879e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7879e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7879e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7879e-113">Not supported.</span></span>  |
|<span data-ttu-id="7879e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7879e-114">Application</span></span> | <span data-ttu-id="7879e-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7879e-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7879e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7879e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7879e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7879e-117">Request headers</span></span>
| <span data-ttu-id="7879e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7879e-118">Header</span></span>       | <span data-ttu-id="7879e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7879e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7879e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7879e-120">Authorization</span></span>  | <span data-ttu-id="7879e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7879e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7879e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7879e-123">Request body</span></span>
<span data-ttu-id="7879e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7879e-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7879e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7879e-125">Response</span></span>
<span data-ttu-id="7879e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7879e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7879e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7879e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7879e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7879e-129">Request</span></span>
<span data-ttu-id="7879e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7879e-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="7879e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7879e-131">Response</span></span>
<span data-ttu-id="7879e-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7879e-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
