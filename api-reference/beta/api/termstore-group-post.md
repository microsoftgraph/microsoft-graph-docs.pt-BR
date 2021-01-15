---
title: Criar grupo
description: Criar um novo objeto de grupo.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: bc7959ec7606a450e9ef920cd96b2550923b03f2
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873903"
---
# <a name="create-group"></a><span data-ttu-id="d5cd0-103">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="d5cd0-103">Create group</span></span>
<span data-ttu-id="d5cd0-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="d5cd0-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5cd0-105">Criar um novo [objeto de](../resources/termstore-group.md) grupo.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-105">Create a new [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5cd0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5cd0-106">Permissions</span></span>
<span data-ttu-id="d5cd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5cd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5cd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5cd0-109">Permission type</span></span>|<span data-ttu-id="d5cd0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5cd0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5cd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5cd0-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d5cd0-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5cd0-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d5cd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5cd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5cd0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-114">Not supported.</span></span>    |
|<span data-ttu-id="d5cd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5cd0-115">Application</span></span> | <span data-ttu-id="d5cd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5cd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5cd0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /termStore/groups
```

## <a name="request-headers"></a><span data-ttu-id="d5cd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5cd0-118">Request headers</span></span>
|<span data-ttu-id="d5cd0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5cd0-119">Name</span></span>|<span data-ttu-id="d5cd0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5cd0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5cd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5cd0-121">Authorization</span></span>|<span data-ttu-id="d5cd0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d5cd0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5cd0-124">Content-Type</span></span>|<span data-ttu-id="d5cd0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5cd0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5cd0-127">Request body</span></span>
<span data-ttu-id="d5cd0-128">No corpo da solicitação, fornece uma representação JSON do [objeto de](../resources/termstore-group.md) grupo.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-128">In the request body, supply a JSON representation of the [group](../resources/termstore-group.md) object.</span></span>

<span data-ttu-id="d5cd0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [grupo.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="d5cd0-129">The following table shows the properties that are required when you create the [group](../resources/termstore-group.md).</span></span>

|<span data-ttu-id="d5cd0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5cd0-130">Property</span></span>|<span data-ttu-id="d5cd0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5cd0-131">Type</span></span>|<span data-ttu-id="d5cd0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5cd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5cd0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d5cd0-133">displayName</span></span>|<span data-ttu-id="d5cd0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5cd0-134">String</span></span>|<span data-ttu-id="d5cd0-135">Nome do grupo a ser criado.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-135">Name of the group to be created.</span></span>|



## <a name="response"></a><span data-ttu-id="d5cd0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5cd0-136">Response</span></span>

<span data-ttu-id="d5cd0-137">Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-137">If successful, this method returns a `201 Created` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5cd0-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d5cd0-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5cd0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5cd0-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="d5cd0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5cd0-140">Response</span></span>
<span data-ttu-id="d5cd0-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d5cd0-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


