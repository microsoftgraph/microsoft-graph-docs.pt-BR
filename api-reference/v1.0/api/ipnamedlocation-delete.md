---
title: Excluir ipNamedLocation
description: Excluir um objeto ipNamedLocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 920ea212232b058153acc4fb58e16ab3a61f85d0
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384453"
---
# <a name="delete-ipnamedlocation"></a><span data-ttu-id="3a90a-103">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3a90a-103">Delete ipNamedLocation</span></span>

<span data-ttu-id="3a90a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a90a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a90a-105">Excluir um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="3a90a-105">Delete an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a90a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a90a-106">Permissions</span></span>

<span data-ttu-id="3a90a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a90a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a90a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a90a-109">Permission type</span></span>                        | <span data-ttu-id="3a90a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a90a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a90a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a90a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a90a-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="3a90a-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="3a90a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a90a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a90a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a90a-114">Not supported.</span></span> |
| <span data-ttu-id="3a90a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a90a-115">Application</span></span>                            | <span data-ttu-id="3a90a-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="3a90a-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a90a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a90a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3a90a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a90a-118">Request headers</span></span>

| <span data-ttu-id="3a90a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3a90a-119">Name</span></span>          | <span data-ttu-id="3a90a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a90a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3a90a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a90a-121">Authorization</span></span> | <span data-ttu-id="3a90a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a90a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a90a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a90a-124">Request body</span></span>

<span data-ttu-id="3a90a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a90a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a90a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a90a-126">Response</span></span>

<span data-ttu-id="3a90a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a90a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a90a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a90a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a90a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a90a-130">Request</span></span>

<span data-ttu-id="3a90a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a90a-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_ipnamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```

### <a name="response"></a><span data-ttu-id="3a90a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a90a-132">Response</span></span>

<span data-ttu-id="3a90a-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a90a-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
