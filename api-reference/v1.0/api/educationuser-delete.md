---
title: Excluir educationUser
description: Exclua um usuário.
ms.openlocfilehash: d9e3cab7d34cdf418b3553d69881bb951217ae22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004491"
---
# <a name="delete-educationuser"></a><span data-ttu-id="2a994-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="2a994-103">Delete educationUser</span></span>

<span data-ttu-id="2a994-104">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="2a994-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="2a994-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a994-105">Permissions</span></span>
<span data-ttu-id="2a994-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a994-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a994-108">Permission type</span></span>      | <span data-ttu-id="2a994-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a994-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a994-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a994-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2a994-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a994-111">Not supported.</span></span>  |
|<span data-ttu-id="2a994-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a994-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2a994-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a994-113">Not supported.</span></span>  |
|<span data-ttu-id="2a994-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a994-114">Application</span></span> | <span data-ttu-id="2a994-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a994-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a994-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a994-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2a994-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a994-117">Request headers</span></span>
| <span data-ttu-id="2a994-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a994-118">Header</span></span>       | <span data-ttu-id="2a994-119">Valor</span><span class="sxs-lookup"><span data-stu-id="2a994-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a994-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a994-120">Authorization</span></span>  | <span data-ttu-id="2a994-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a994-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a994-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a994-123">Request body</span></span>
<span data-ttu-id="2a994-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a994-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2a994-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a994-125">Response</span></span>
<span data-ttu-id="2a994-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a994-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a994-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a994-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a994-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a994-129">Request</span></span>
<span data-ttu-id="2a994-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a994-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="2a994-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a994-131">Response</span></span>
<span data-ttu-id="2a994-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a994-132">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->