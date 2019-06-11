---
title: Excluir grupo-API do Microsoft Graph
description: Descreve o método Delete do recurso de grupo (entidade) da API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9d0680adc000f089ba54d3af7b1e84523025d367
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812821"
---
# <a name="delete-group"></a><span data-ttu-id="d79ab-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="d79ab-103">Delete group</span></span>

<span data-ttu-id="d79ab-104">Excluir o grupo.</span><span class="sxs-lookup"><span data-stu-id="d79ab-104">Delete group.</span></span>  

<span data-ttu-id="d79ab-105">Quando excluídos, os grupos do Office 365 são movidos para um contêiner temporário e podem ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="d79ab-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="d79ab-106">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="d79ab-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="d79ab-107">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="d79ab-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="d79ab-108">Isso se aplica apenas aos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d79ab-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d79ab-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d79ab-109">Permissions</span></span>

<span data-ttu-id="d79ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d79ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d79ab-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d79ab-112">Permission type</span></span>      | <span data-ttu-id="d79ab-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d79ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d79ab-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d79ab-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d79ab-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d79ab-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="d79ab-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d79ab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d79ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d79ab-117">Not supported.</span></span>    |
|<span data-ttu-id="d79ab-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d79ab-118">Application</span></span> | <span data-ttu-id="d79ab-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79ab-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d79ab-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d79ab-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d79ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d79ab-121">Request headers</span></span>

| <span data-ttu-id="d79ab-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d79ab-122">Name</span></span>       | <span data-ttu-id="d79ab-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d79ab-123">Type</span></span> | <span data-ttu-id="d79ab-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d79ab-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d79ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d79ab-125">Authorization</span></span>  | <span data-ttu-id="d79ab-126">string</span><span class="sxs-lookup"><span data-stu-id="d79ab-126">string</span></span>  | <span data-ttu-id="d79ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d79ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d79ab-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d79ab-129">Request body</span></span>

<span data-ttu-id="d79ab-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d79ab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d79ab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d79ab-131">Response</span></span>

<span data-ttu-id="d79ab-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d79ab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d79ab-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d79ab-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d79ab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d79ab-135">Request</span></span>

<span data-ttu-id="d79ab-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d79ab-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

### <a name="response"></a><span data-ttu-id="d79ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d79ab-137">Response</span></span>

<span data-ttu-id="d79ab-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d79ab-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d79ab-139">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="d79ab-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d79ab-140">C#</span><span class="sxs-lookup"><span data-stu-id="d79ab-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d79ab-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d79ab-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
