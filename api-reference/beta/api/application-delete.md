---
title: Excluir aplicativo
description: Exclui um aplicativo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 58b27088e5fc53b1be5f015aa2f7b194ab9825d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322639"
---
# <a name="delete-application"></a><span data-ttu-id="63026-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="63026-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63026-104">Exclui um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63026-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="63026-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="63026-105">Permissions</span></span>
<span data-ttu-id="63026-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63026-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63026-108">Permission type</span></span>      | <span data-ttu-id="63026-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63026-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63026-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63026-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63026-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63026-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63026-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63026-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63026-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63026-113">Not supported.</span></span>    |
|<span data-ttu-id="63026-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63026-114">Application</span></span> | <span data-ttu-id="63026-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63026-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63026-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63026-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63026-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63026-117">Request headers</span></span>
| <span data-ttu-id="63026-118">Nome</span><span class="sxs-lookup"><span data-stu-id="63026-118">Name</span></span>       | <span data-ttu-id="63026-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="63026-119">Type</span></span> | <span data-ttu-id="63026-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63026-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="63026-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="63026-121">Authorization</span></span>  | <span data-ttu-id="63026-122">string</span><span class="sxs-lookup"><span data-stu-id="63026-122">string</span></span>  | <span data-ttu-id="63026-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63026-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63026-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63026-125">Request body</span></span>
<span data-ttu-id="63026-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63026-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63026-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="63026-127">Response</span></span>

<span data-ttu-id="63026-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63026-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63026-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63026-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63026-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63026-131">Request</span></span>
<span data-ttu-id="63026-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63026-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="63026-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="63026-133">Response</span></span>
<span data-ttu-id="63026-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63026-134">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
