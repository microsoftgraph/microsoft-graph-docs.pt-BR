---
title: Excluir educationSchool
description: Exclua uma escola.
ms.openlocfilehash: 48516780c0132012b8b7f2d8aa9295af7ade0711
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006812"
---
# <a name="delete-educationschool"></a><span data-ttu-id="de550-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="de550-103">Delete educationSchool</span></span>

<span data-ttu-id="de550-104">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="de550-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="de550-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="de550-105">Permissions</span></span>
<span data-ttu-id="de550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de550-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de550-108">Permission type</span></span>      | <span data-ttu-id="de550-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de550-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de550-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de550-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="de550-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de550-111">Not supported.</span></span>  |
|<span data-ttu-id="de550-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de550-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="de550-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de550-113">Not supported.</span></span>  |
|<span data-ttu-id="de550-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de550-114">Application</span></span> | <span data-ttu-id="de550-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de550-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="de550-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de550-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="de550-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de550-117">Request headers</span></span>
| <span data-ttu-id="de550-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de550-118">Header</span></span>       | <span data-ttu-id="de550-119">Valor</span><span class="sxs-lookup"><span data-stu-id="de550-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de550-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="de550-120">Authorization</span></span>  | <span data-ttu-id="de550-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de550-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de550-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de550-123">Request body</span></span>
<span data-ttu-id="de550-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de550-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="de550-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="de550-125">Response</span></span>
<span data-ttu-id="de550-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de550-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de550-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de550-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de550-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de550-129">Request</span></span>
<span data-ttu-id="de550-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de550-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="de550-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="de550-131">Response</span></span>
<span data-ttu-id="de550-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de550-132">The following is an example of the response.</span></span> 

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