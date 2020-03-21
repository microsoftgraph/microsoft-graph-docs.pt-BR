---
title: Excluir printerShare
description: Excluir um compartilhamento de impressora (descompartilhar a impressora associada). Não é possível desfazer a ação. Se a impressora for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a impressora deverá descobrir e reinstalá-la.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 534dc61037efd99f92100c87bc911cdea6dfb6a5
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895547"
---
# <a name="delete-printershare"></a><span data-ttu-id="e41d0-105">Excluir printerShare</span><span class="sxs-lookup"><span data-stu-id="e41d0-105">Delete printerShare</span></span>

<span data-ttu-id="e41d0-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e41d0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e41d0-107">Excluir um compartilhamento de impressora (descompartilhar a [impressora](../resources/printer.md)associada).</span><span class="sxs-lookup"><span data-stu-id="e41d0-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="e41d0-108">Não é possível desfazer a ação.</span><span class="sxs-lookup"><span data-stu-id="e41d0-108">This action cannot be undone.</span></span> <span data-ttu-id="e41d0-109">Se a [impressora](../resources/printer.md) for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a [impressora](../resources/printer.md) deverá descobrir e reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="e41d0-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="e41d0-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e41d0-110">Permissions</span></span>
<span data-ttu-id="e41d0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e41d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e41d0-113">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="e41d0-113">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e41d0-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e41d0-114">Permission type</span></span> | <span data-ttu-id="e41d0-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e41d0-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e41d0-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e41d0-116">Delegated (work or school account)</span></span>| <span data-ttu-id="e41d0-117">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="e41d0-117">Users.Read.All</span></span> |
|<span data-ttu-id="e41d0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e41d0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e41d0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e41d0-119">Not Supported.</span></span>|
|<span data-ttu-id="e41d0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e41d0-120">Application</span></span>|<span data-ttu-id="e41d0-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e41d0-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e41d0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e41d0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="e41d0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e41d0-123">Request headers</span></span>
| <span data-ttu-id="e41d0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e41d0-124">Name</span></span>          | <span data-ttu-id="e41d0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e41d0-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e41d0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e41d0-126">Authorization</span></span> | <span data-ttu-id="e41d0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e41d0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e41d0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e41d0-129">Request body</span></span>
<span data-ttu-id="e41d0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e41d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e41d0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e41d0-131">Response</span></span>
<span data-ttu-id="e41d0-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e41d0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e41d0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e41d0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e41d0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e41d0-135">Request</span></span>
<span data-ttu-id="e41d0-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e41d0-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShares/{id}
```
##### <a name="response"></a><span data-ttu-id="e41d0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e41d0-137">Response</span></span>
<span data-ttu-id="e41d0-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e41d0-138">The following is an example of the response.</span></span>
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
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->