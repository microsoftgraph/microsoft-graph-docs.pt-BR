---
title: Excluir allowedUser
description: Revoga o acesso do usuário especificado para enviar trabalhos de impressão ao compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9812f462561a04ffd88e0e927f58b34d963173d4
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807069"
---
# <a name="delete-alloweduser"></a><span data-ttu-id="bb965-103">Excluir allowedUser</span><span class="sxs-lookup"><span data-stu-id="bb965-103">Delete allowedUser</span></span>

<span data-ttu-id="bb965-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb965-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb965-105">Revoga o acesso do usuário especificado para enviar trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="bb965-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb965-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb965-106">Permissions</span></span>
<span data-ttu-id="bb965-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb965-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bb965-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="bb965-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="bb965-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb965-110">Permission type</span></span> | <span data-ttu-id="bb965-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb965-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bb965-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb965-112">Delegated (work or school account)</span></span>| <span data-ttu-id="bb965-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="bb965-113">Users.Read.All</span></span> |
|<span data-ttu-id="bb965-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb965-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb965-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb965-115">Not Supported.</span></span>|
|<span data-ttu-id="bb965-116">Application</span><span class="sxs-lookup"><span data-stu-id="bb965-116">Application</span></span>|<span data-ttu-id="bb965-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb965-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb965-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb965-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShare/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bb965-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb965-119">Request headers</span></span>
| <span data-ttu-id="bb965-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bb965-120">Name</span></span>          | <span data-ttu-id="bb965-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb965-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb965-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb965-122">Authorization</span></span> | <span data-ttu-id="bb965-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb965-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb965-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb965-125">Request body</span></span>
<span data-ttu-id="bb965-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb965-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb965-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb965-127">Response</span></span>
<span data-ttu-id="bb965-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb965-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb965-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb965-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb965-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb965-131">Request</span></span>
<span data-ttu-id="bb965-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb965-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShare/{id}/allowedUsers/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="bb965-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb965-133">Response</span></span>
<span data-ttu-id="bb965-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb965-134">The following is an example of the response.</span></span>
><span data-ttu-id="bb965-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb965-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
