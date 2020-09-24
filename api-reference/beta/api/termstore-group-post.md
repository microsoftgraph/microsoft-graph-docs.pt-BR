---
title: Criar grupo
description: Criar um novo objeto de grupo.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 314795b1edad398a093b3c1bbfc401c0ef450c23
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258447"
---
# <a name="create-group"></a><span data-ttu-id="c6d44-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="c6d44-103">Create group</span></span>
<span data-ttu-id="c6d44-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="c6d44-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6d44-105">Criar um novo objeto de [grupo](../resources/termstore-group.md) .</span><span class="sxs-lookup"><span data-stu-id="c6d44-105">Create a new [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6d44-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6d44-106">Permissions</span></span>
<span data-ttu-id="c6d44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6d44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d44-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6d44-109">Permission type</span></span>|<span data-ttu-id="c6d44-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6d44-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6d44-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6d44-111">Delegated (work or school account)</span></span> |<span data-ttu-id="c6d44-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6d44-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="c6d44-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6d44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6d44-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6d44-114">Not supported.</span></span>    |
|<span data-ttu-id="c6d44-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6d44-115">Application</span></span> | <span data-ttu-id="c6d44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6d44-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6d44-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6d44-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /termStore/groups
```

## <a name="request-headers"></a><span data-ttu-id="c6d44-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d44-118">Request headers</span></span>
|<span data-ttu-id="c6d44-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c6d44-119">Name</span></span>|<span data-ttu-id="c6d44-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6d44-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c6d44-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6d44-121">Authorization</span></span>|<span data-ttu-id="c6d44-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6d44-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c6d44-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6d44-124">Content-Type</span></span>|<span data-ttu-id="c6d44-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6d44-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d44-127">Request body</span></span>
<span data-ttu-id="c6d44-128">No corpo da solicitação, forneça uma representação JSON do objeto [Group](../resources/termstore-group.md) .</span><span class="sxs-lookup"><span data-stu-id="c6d44-128">In the request body, supply a JSON representation of the [group](../resources/termstore-group.md) object.</span></span>

<span data-ttu-id="c6d44-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [grupo](../resources/termstore-group.md).</span><span class="sxs-lookup"><span data-stu-id="c6d44-129">The following table shows the properties that are required when you create the [group](../resources/termstore-group.md).</span></span>

|<span data-ttu-id="c6d44-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6d44-130">Property</span></span>|<span data-ttu-id="c6d44-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6d44-131">Type</span></span>|<span data-ttu-id="c6d44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6d44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6d44-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c6d44-133">displayName</span></span>|<span data-ttu-id="c6d44-134">String</span><span class="sxs-lookup"><span data-stu-id="c6d44-134">String</span></span>|<span data-ttu-id="c6d44-135">Nome do grupo a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c6d44-135">Name of the group to be created.</span></span>|



## <a name="response"></a><span data-ttu-id="c6d44-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6d44-136">Response</span></span>

<span data-ttu-id="c6d44-137">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6d44-137">If successful, this method returns a `201 Created` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6d44-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c6d44-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c6d44-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d44-139">Request</span></span>
<!-- {
  "blockType": "request",
  "displayName": "myGroup"
}-->

``` http
POST https://graph.microsoft.com/beta/termStore/groups
Content-Type: application/json
Content-length: 135

{
  "displayName" : "myGroup"
}
```


### <a name="response"></a><span data-ttu-id="c6d44-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6d44-140">Response</span></span>
<span data-ttu-id="c6d44-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c6d44-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "85825593-5593-8582-9355-828593558285",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "displayName": "myGroup"  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termGroup",
  "suppressions": [
  ]
}
-->


