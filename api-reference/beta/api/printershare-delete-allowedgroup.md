---
title: Excluir o permitido
description: Revoga o acesso do grupo especificado para enviar trabalhos de impressão ao compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e6c3fb214126d4414ed35d6ba58a52acc6b65bab
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216617"
---
# <a name="delete-allowedgroup"></a><span data-ttu-id="c8be6-103">Excluir o permitido</span><span class="sxs-lookup"><span data-stu-id="c8be6-103">Delete allowedGroup</span></span>

<span data-ttu-id="c8be6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8be6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8be6-105">Revoga o acesso do grupo especificado para enviar trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="c8be6-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8be6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8be6-106">Permissions</span></span>
<span data-ttu-id="c8be6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8be6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c8be6-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="c8be6-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c8be6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8be6-110">Permission type</span></span> | <span data-ttu-id="c8be6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8be6-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c8be6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8be6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c8be6-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="c8be6-113">Users.Read.All</span></span> |
|<span data-ttu-id="c8be6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8be6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8be6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8be6-115">Not Supported.</span></span>|
|<span data-ttu-id="c8be6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8be6-116">Application</span></span>|<span data-ttu-id="c8be6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8be6-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8be6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8be6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c8be6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8be6-119">Request headers</span></span>
| <span data-ttu-id="c8be6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c8be6-120">Name</span></span>          | <span data-ttu-id="c8be6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8be6-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c8be6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8be6-122">Authorization</span></span> | <span data-ttu-id="c8be6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8be6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8be6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8be6-125">Request body</span></span>
<span data-ttu-id="c8be6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8be6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8be6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8be6-127">Response</span></span>
<span data-ttu-id="c8be6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8be6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8be6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8be6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8be6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8be6-131">Request</span></span>
<span data-ttu-id="c8be6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8be6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroup/{id}/$ref
```
##### <a name="response"></a><span data-ttu-id="c8be6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8be6-133">Response</span></span>
<span data-ttu-id="c8be6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8be6-134">The following is an example of the response.</span></span>
><span data-ttu-id="c8be6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8be6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->