---
title: Excluir grupo-API do Microsoft Graph
description: Descreve o método Delete do recurso de grupo (entidade) da API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 836f2c647fd9894a7d39bba80e5f15f3f11ef81f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255861"
---
# <a name="delete-group"></a><span data-ttu-id="a507d-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="a507d-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a507d-104">Exclui um grupo.</span><span class="sxs-lookup"><span data-stu-id="a507d-104">Deletes a group.</span></span>  

<span data-ttu-id="a507d-105">Quando excluídos, os grupos do Office 365 são movidos para um contêiner temporário e podem ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="a507d-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="a507d-106">Após esse tempo, elas serão excluídas permanentemente.</span><span class="sxs-lookup"><span data-stu-id="a507d-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="a507d-107">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a507d-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="a507d-108">Isso se aplica apenas aos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a507d-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="a507d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a507d-109">Permissions</span></span>

<span data-ttu-id="a507d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a507d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a507d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a507d-112">Permission type</span></span>      | <span data-ttu-id="a507d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a507d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a507d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a507d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a507d-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a507d-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a507d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a507d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a507d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a507d-117">Not supported.</span></span>    |
|<span data-ttu-id="a507d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a507d-118">Application</span></span> | <span data-ttu-id="a507d-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a507d-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a507d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a507d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a507d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a507d-121">Request headers</span></span>

| <span data-ttu-id="a507d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a507d-122">Name</span></span>       | <span data-ttu-id="a507d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a507d-123">Type</span></span> | <span data-ttu-id="a507d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a507d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a507d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a507d-125">Authorization</span></span>  | <span data-ttu-id="a507d-126">string</span><span class="sxs-lookup"><span data-stu-id="a507d-126">string</span></span>  | <span data-ttu-id="a507d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a507d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a507d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a507d-129">Request body</span></span>

<span data-ttu-id="a507d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a507d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a507d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a507d-131">Response</span></span>

<span data-ttu-id="a507d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a507d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a507d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a507d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a507d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a507d-135">Request</span></span>

<span data-ttu-id="a507d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a507d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="a507d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a507d-137">Response</span></span>

<span data-ttu-id="a507d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a507d-138">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
