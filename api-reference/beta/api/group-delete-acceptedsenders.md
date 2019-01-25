---
title: Remover acceptedSender
description: 'Remova um usuário ou grupo da lista acceptedSenders. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a3406c028990b7b5989036f4173cf86f257b4f03
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520687"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="8e00d-103">Remover acceptedSender</span><span class="sxs-lookup"><span data-stu-id="8e00d-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e00d-104">Remova um usuário ou grupo da lista acceptedSenders.</span><span class="sxs-lookup"><span data-stu-id="8e00d-104">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8e00d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e00d-105">Permissions</span></span>
<span data-ttu-id="8e00d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e00d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e00d-108">Permission type</span></span>                        | <span data-ttu-id="8e00d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e00d-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="8e00d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e00d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e00d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e00d-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="8e00d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e00d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e00d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e00d-113">Not supported.</span></span>|
| <span data-ttu-id="8e00d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e00d-114">Application</span></span>                            | <span data-ttu-id="8e00d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e00d-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e00d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e00d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="8e00d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e00d-117">Request headers</span></span>
| <span data-ttu-id="8e00d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e00d-118">Header</span></span>         | <span data-ttu-id="8e00d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8e00d-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="8e00d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e00d-120">Authorization</span></span>  | <span data-ttu-id="8e00d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e00d-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="8e00d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e00d-123">Request body</span></span>
<span data-ttu-id="8e00d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e00d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e00d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e00d-125">Response</span></span>
<span data-ttu-id="8e00d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e00d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e00d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e00d-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8e00d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e00d-129">Request</span></span>
<span data-ttu-id="8e00d-130">Estes são alguns exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e00d-130">The following are a couple of examples of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="8e00d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e00d-131">Response</span></span>
<span data-ttu-id="8e00d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e00d-132">The following is an example of the response.</span></span> 

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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-acceptedsenders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
