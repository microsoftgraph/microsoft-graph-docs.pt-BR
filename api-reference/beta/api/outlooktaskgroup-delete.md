---
title: Excluir outlookTaskGroup
description: Exclua o outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cfe3c88adf821ca8a5643cdafd5719b5fbb4d40e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539970"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="9b904-103">Excluir outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9b904-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b904-104">Exclua o [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9b904-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9b904-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b904-105">Permissions</span></span>
<span data-ttu-id="9b904-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b904-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b904-108">Permission type</span></span>      | <span data-ttu-id="9b904-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b904-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b904-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b904-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b904-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b904-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9b904-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b904-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b904-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b904-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9b904-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b904-114">Application</span></span> | <span data-ttu-id="9b904-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b904-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b904-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b904-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9b904-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b904-117">Request headers</span></span>
| <span data-ttu-id="9b904-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9b904-118">Name</span></span>       | <span data-ttu-id="9b904-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b904-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b904-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b904-120">Authorization</span></span>  | <span data-ttu-id="9b904-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b904-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b904-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b904-123">Request body</span></span>
<span data-ttu-id="9b904-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b904-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b904-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b904-125">Response</span></span>

<span data-ttu-id="9b904-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b904-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b904-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b904-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b904-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b904-129">Request</span></span>
<span data-ttu-id="9b904-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b904-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="9b904-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b904-131">Response</span></span>
<span data-ttu-id="9b904-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b904-132">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
