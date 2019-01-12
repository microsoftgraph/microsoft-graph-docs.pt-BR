---
title: Excluir educationClass
description: Exclua uma aula. Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9b25e95dfa109ef48d67374ba7569a32af22ba50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935063"
---
# <a name="delete-educationclass"></a><span data-ttu-id="24e62-104">Excluir educationClass</span><span class="sxs-lookup"><span data-stu-id="24e62-104">Delete educationClass</span></span>

> <span data-ttu-id="24e62-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="24e62-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24e62-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="24e62-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24e62-107">Exclua uma aula.</span><span class="sxs-lookup"><span data-stu-id="24e62-107">Delete a class.</span></span> <span data-ttu-id="24e62-108">Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.</span><span class="sxs-lookup"><span data-stu-id="24e62-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="24e62-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="24e62-109">Permissions</span></span>
<span data-ttu-id="24e62-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24e62-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24e62-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24e62-112">Permission type</span></span>      | <span data-ttu-id="24e62-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24e62-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24e62-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24e62-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="24e62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24e62-115">Not supported.</span></span>  |
|<span data-ttu-id="24e62-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24e62-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="24e62-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24e62-117">Not supported.</span></span>  |
|<span data-ttu-id="24e62-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24e62-118">Application</span></span> | <span data-ttu-id="24e62-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24e62-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="24e62-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24e62-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="24e62-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24e62-121">Request headers</span></span>
| <span data-ttu-id="24e62-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24e62-122">Header</span></span>       | <span data-ttu-id="24e62-123">Valor</span><span class="sxs-lookup"><span data-stu-id="24e62-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24e62-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="24e62-124">Authorization</span></span>  | <span data-ttu-id="24e62-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24e62-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24e62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24e62-127">Request body</span></span>
<span data-ttu-id="24e62-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24e62-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="24e62-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="24e62-129">Response</span></span>
<span data-ttu-id="24e62-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24e62-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24e62-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24e62-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24e62-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24e62-133">Request</span></span>
<span data-ttu-id="24e62-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24e62-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="24e62-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="24e62-135">Response</span></span>
<span data-ttu-id="24e62-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24e62-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
