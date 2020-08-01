---
title: Excluir termo
description: Excluir um objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e9af0729c07896a707c35b7cd3e4eb3e122e5e10
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539165"
---
# <a name="delete-term"></a><span data-ttu-id="69d61-103">Excluir termo</span><span class="sxs-lookup"><span data-stu-id="69d61-103">Delete term</span></span>
<span data-ttu-id="69d61-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="69d61-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69d61-105">Excluir um objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="69d61-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69d61-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="69d61-106">Permissions</span></span>
<span data-ttu-id="69d61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69d61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69d61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69d61-109">Permission type</span></span>|<span data-ttu-id="69d61-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69d61-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69d61-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69d61-111">Delegated (work or school account)</span></span> |<span data-ttu-id="69d61-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69d61-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="69d61-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69d61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69d61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69d61-114">Not supported.</span></span>    |
|<span data-ttu-id="69d61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69d61-115">Application</span></span> | <span data-ttu-id="69d61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69d61-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="69d61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69d61-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="69d61-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69d61-118">Request headers</span></span>
|<span data-ttu-id="69d61-119">Nome</span><span class="sxs-lookup"><span data-stu-id="69d61-119">Name</span></span>|<span data-ttu-id="69d61-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69d61-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69d61-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="69d61-121">Authorization</span></span>|<span data-ttu-id="69d61-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69d61-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69d61-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69d61-124">Request body</span></span>
<span data-ttu-id="69d61-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69d61-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69d61-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="69d61-126">Response</span></span>

<span data-ttu-id="69d61-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69d61-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69d61-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="69d61-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69d61-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69d61-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```


### <a name="response"></a><span data-ttu-id="69d61-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="69d61-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete term",
  "suppressions": [
  ]
}
-->
