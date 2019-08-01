---
title: Excluir grupo-API do Microsoft Graph
description: Descreve o método Delete do recurso de grupo (entidade) da API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 95638630fd95220760cce6766edbef5dc84cb544
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014967"
---
# <a name="delete-group"></a><span data-ttu-id="488cc-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="488cc-103">Delete group</span></span>

<span data-ttu-id="488cc-104">Excluir o grupo.</span><span class="sxs-lookup"><span data-stu-id="488cc-104">Delete group.</span></span>  

<span data-ttu-id="488cc-105">Quando excluídos, os grupos do Office 365 são movidos para um contêiner temporário e podem ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="488cc-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="488cc-106">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="488cc-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="488cc-107">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="488cc-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="488cc-108">Isso se aplica apenas aos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="488cc-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="488cc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="488cc-109">Permissions</span></span>

<span data-ttu-id="488cc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="488cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="488cc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="488cc-112">Permission type</span></span>      | <span data-ttu-id="488cc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="488cc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="488cc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="488cc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="488cc-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="488cc-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="488cc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="488cc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="488cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="488cc-117">Not supported.</span></span>    |
|<span data-ttu-id="488cc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="488cc-118">Application</span></span> | <span data-ttu-id="488cc-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="488cc-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="488cc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="488cc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="488cc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="488cc-121">Request headers</span></span>

| <span data-ttu-id="488cc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="488cc-122">Name</span></span>       | <span data-ttu-id="488cc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="488cc-123">Type</span></span> | <span data-ttu-id="488cc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="488cc-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="488cc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="488cc-125">Authorization</span></span>  | <span data-ttu-id="488cc-126">string</span><span class="sxs-lookup"><span data-stu-id="488cc-126">string</span></span>  | <span data-ttu-id="488cc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="488cc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="488cc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="488cc-129">Request body</span></span>

<span data-ttu-id="488cc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="488cc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="488cc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="488cc-131">Response</span></span>

<span data-ttu-id="488cc-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="488cc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="488cc-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="488cc-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="488cc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="488cc-135">Request</span></span>

<span data-ttu-id="488cc-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="488cc-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="488cc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="488cc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="488cc-138">C#</span><span class="sxs-lookup"><span data-stu-id="488cc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="488cc-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="488cc-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="488cc-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="488cc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="488cc-141">Java</span><span class="sxs-lookup"><span data-stu-id="488cc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="488cc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="488cc-142">Response</span></span>

<span data-ttu-id="488cc-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="488cc-143">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
