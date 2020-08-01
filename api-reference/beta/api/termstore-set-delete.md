---
title: Excluir conjunto
description: Excluir um objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 83b48322c28330d22047a15cc488d276281fcc71
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539138"
---
# <a name="delete-set"></a><span data-ttu-id="79257-103">Excluir conjunto</span><span class="sxs-lookup"><span data-stu-id="79257-103">Delete set</span></span>
<span data-ttu-id="79257-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="79257-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79257-105">Excluir um objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="79257-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79257-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79257-106">Permissions</span></span>
<span data-ttu-id="79257-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79257-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79257-109">Permission type</span></span>|<span data-ttu-id="79257-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79257-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79257-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79257-111">Delegated (work or school account)</span></span> |<span data-ttu-id="79257-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79257-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="79257-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79257-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79257-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79257-114">Not supported.</span></span>    |
|<span data-ttu-id="79257-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79257-115">Application</span></span> | <span data-ttu-id="79257-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79257-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="79257-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79257-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="79257-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79257-118">Request headers</span></span>
|<span data-ttu-id="79257-119">Nome</span><span class="sxs-lookup"><span data-stu-id="79257-119">Name</span></span>|<span data-ttu-id="79257-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79257-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79257-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79257-121">Authorization</span></span>|<span data-ttu-id="79257-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79257-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79257-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79257-124">Request body</span></span>
<span data-ttu-id="79257-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79257-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79257-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="79257-126">Response</span></span>

<span data-ttu-id="79257-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79257-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="79257-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79257-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79257-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79257-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```


### <a name="response"></a><span data-ttu-id="79257-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="79257-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->
