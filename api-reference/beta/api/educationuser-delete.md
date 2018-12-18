---
title: Excluir educationUser
description: Exclua um usuário.
author: mmast-msft
ms.openlocfilehash: e74b45a1de58cc02fdd559821812aebcc9292fc1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362808"
---
# <a name="delete-educationuser"></a><span data-ttu-id="ed238-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="ed238-103">Delete educationUser</span></span>

> <span data-ttu-id="ed238-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed238-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed238-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed238-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed238-106">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="ed238-106">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="ed238-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed238-107">Permissions</span></span>
<span data-ttu-id="ed238-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed238-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed238-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed238-110">Permission type</span></span>      | <span data-ttu-id="ed238-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed238-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed238-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed238-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed238-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed238-113">Not supported.</span></span>  |
|<span data-ttu-id="ed238-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed238-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ed238-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed238-115">Not supported.</span></span>  |
|<span data-ttu-id="ed238-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed238-116">Application</span></span> | <span data-ttu-id="ed238-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed238-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed238-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed238-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ed238-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed238-119">Request headers</span></span>
| <span data-ttu-id="ed238-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed238-120">Header</span></span>       | <span data-ttu-id="ed238-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed238-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed238-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed238-122">Authorization</span></span>  | <span data-ttu-id="ed238-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed238-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed238-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed238-125">Request body</span></span>
<span data-ttu-id="ed238-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed238-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ed238-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed238-127">Response</span></span>
<span data-ttu-id="ed238-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed238-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed238-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed238-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed238-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed238-131">Request</span></span>
<span data-ttu-id="ed238-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed238-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
##### <a name="response"></a><span data-ttu-id="ed238-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed238-133">Response</span></span>
<span data-ttu-id="ed238-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed238-134">The following is an example of the response.</span></span> 
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