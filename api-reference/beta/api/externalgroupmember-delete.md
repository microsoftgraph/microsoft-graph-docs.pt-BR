---
title: Excluir externalGroupMember
description: Excluir um objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 3347b51ba6b3fa5928e08ea85540cc0e634a1a7a
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193815"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="d8b16-103">Excluir externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="d8b16-103">Delete externalGroupMember</span></span>

<span data-ttu-id="d8b16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8b16-105">Excluir um objeto [externalGroupMember](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="d8b16-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8b16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8b16-106">Permissions</span></span>

<span data-ttu-id="d8b16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8b16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8b16-109">Permission type</span></span>                        | <span data-ttu-id="d8b16-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8b16-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d8b16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8b16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8b16-112">Incompatível</span><span class="sxs-lookup"><span data-stu-id="d8b16-112">Not supported</span></span>                               |
| <span data-ttu-id="d8b16-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8b16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8b16-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8b16-114">Not supported</span></span>                               |
| <span data-ttu-id="d8b16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8b16-115">Application</span></span>                            | <span data-ttu-id="d8b16-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b16-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="d8b16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8b16-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="d8b16-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b16-118">Request headers</span></span>

| <span data-ttu-id="d8b16-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d8b16-119">Name</span></span>          | <span data-ttu-id="d8b16-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b16-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d8b16-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8b16-121">Authorization</span></span> | <span data-ttu-id="d8b16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8b16-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8b16-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b16-124">Request body</span></span>

<span data-ttu-id="d8b16-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8b16-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8b16-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8b16-126">Response</span></span>

<span data-ttu-id="d8b16-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d8b16-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d8b16-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d8b16-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8b16-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b16-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d8b16-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8b16-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
