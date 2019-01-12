---
title: Excluir educationUser
description: Exclua um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2d07a44cffc70e5ed247b80861e1660a105b1689
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930779"
---
# <a name="delete-educationuser"></a><span data-ttu-id="301f0-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="301f0-103">Delete educationUser</span></span>

> <span data-ttu-id="301f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="301f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="301f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="301f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="301f0-106">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="301f0-106">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="301f0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="301f0-107">Permissions</span></span>
<span data-ttu-id="301f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="301f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="301f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="301f0-110">Permission type</span></span>      | <span data-ttu-id="301f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="301f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="301f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="301f0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="301f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="301f0-113">Not supported.</span></span>  |
|<span data-ttu-id="301f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="301f0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="301f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="301f0-115">Not supported.</span></span>  |
|<span data-ttu-id="301f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="301f0-116">Application</span></span> | <span data-ttu-id="301f0-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="301f0-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="301f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="301f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="301f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="301f0-119">Request headers</span></span>
| <span data-ttu-id="301f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="301f0-120">Header</span></span>       | <span data-ttu-id="301f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="301f0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="301f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="301f0-122">Authorization</span></span>  | <span data-ttu-id="301f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="301f0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="301f0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="301f0-125">Request body</span></span>
<span data-ttu-id="301f0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="301f0-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="301f0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="301f0-127">Response</span></span>
<span data-ttu-id="301f0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="301f0-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="301f0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="301f0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="301f0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="301f0-131">Request</span></span>
<span data-ttu-id="301f0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="301f0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
##### <a name="response"></a><span data-ttu-id="301f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="301f0-133">Response</span></span>
<span data-ttu-id="301f0-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="301f0-134">The following is an example of the response.</span></span> 
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
