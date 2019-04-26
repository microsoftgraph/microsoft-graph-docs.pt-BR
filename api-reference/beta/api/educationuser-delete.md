---
title: Excluir educationUser
description: Exclua um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7028ee71cbbd0b4166ea046a2ceae2f156115ddf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322985"
---
# <a name="delete-educationuser"></a><span data-ttu-id="e35d0-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="e35d0-103">Delete educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35d0-104">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="e35d0-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="e35d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e35d0-105">Permissions</span></span>
<span data-ttu-id="e35d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e35d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e35d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e35d0-108">Permission type</span></span>      | <span data-ttu-id="e35d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e35d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e35d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e35d0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e35d0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e35d0-111">Not supported.</span></span>  |
|<span data-ttu-id="e35d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e35d0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e35d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e35d0-113">Not supported.</span></span>  |
|<span data-ttu-id="e35d0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e35d0-114">Application</span></span> | <span data-ttu-id="e35d0-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e35d0-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e35d0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e35d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e35d0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e35d0-117">Request headers</span></span>
| <span data-ttu-id="e35d0-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e35d0-118">Header</span></span>       | <span data-ttu-id="e35d0-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e35d0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e35d0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e35d0-120">Authorization</span></span>  | <span data-ttu-id="e35d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e35d0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e35d0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e35d0-123">Request body</span></span>
<span data-ttu-id="e35d0-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e35d0-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e35d0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35d0-125">Response</span></span>
<span data-ttu-id="e35d0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e35d0-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e35d0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e35d0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e35d0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e35d0-129">Request</span></span>
<span data-ttu-id="e35d0-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e35d0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
##### <a name="response"></a><span data-ttu-id="e35d0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35d0-131">Response</span></span>
<span data-ttu-id="e35d0-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e35d0-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
