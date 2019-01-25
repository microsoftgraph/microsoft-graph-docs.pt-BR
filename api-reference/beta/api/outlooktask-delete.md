---
title: Excluir outlookTask
description: Exclua a tarefa especificada do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45660f5bb4a2c74fccb5b618dc30f7d331f558bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517971"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="cdd15-103">Excluir outlookTask</span><span class="sxs-lookup"><span data-stu-id="cdd15-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdd15-104">Exclua a tarefa especificada do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cdd15-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd15-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdd15-105">Permissions</span></span>

<span data-ttu-id="cdd15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd15-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdd15-108">Permission type</span></span>      | <span data-ttu-id="cdd15-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdd15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd15-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdd15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd15-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdd15-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cdd15-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdd15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd15-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdd15-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cdd15-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdd15-114">Application</span></span> | <span data-ttu-id="cdd15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdd15-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdd15-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd15-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cdd15-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd15-117">Request headers</span></span>

| <span data-ttu-id="cdd15-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cdd15-118">Name</span></span>       | <span data-ttu-id="cdd15-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdd15-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cdd15-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdd15-120">Authorization</span></span>  | <span data-ttu-id="cdd15-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdd15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdd15-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd15-123">Request body</span></span>

<span data-ttu-id="cdd15-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdd15-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdd15-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd15-125">Response</span></span>

<span data-ttu-id="cdd15-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd15-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdd15-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdd15-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdd15-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd15-129">Request</span></span>

<span data-ttu-id="cdd15-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdd15-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```

### <a name="response"></a><span data-ttu-id="cdd15-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd15-131">Response</span></span>

<span data-ttu-id="cdd15-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd15-132">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
