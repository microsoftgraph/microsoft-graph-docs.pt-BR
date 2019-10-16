---
title: Excluir certificateBasedAuthConfiguration
description: Exclua certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8bab6d42550e009897db42a2556e687059330000
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539236"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="97405-103">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="97405-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="97405-104">Excluir um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="97405-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97405-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97405-105">Permissions</span></span>

<span data-ttu-id="97405-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97405-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97405-108">Permission type</span></span>                        | <span data-ttu-id="97405-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97405-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97405-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97405-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97405-111">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="97405-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="97405-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97405-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97405-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97405-113">Not supported.</span></span> |
| <span data-ttu-id="97405-114">Application</span><span class="sxs-lookup"><span data-stu-id="97405-114">Application</span></span>    | <span data-ttu-id="97405-115">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="97405-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97405-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97405-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97405-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97405-117">Request headers</span></span>

| <span data-ttu-id="97405-118">Nome</span><span class="sxs-lookup"><span data-stu-id="97405-118">Name</span></span>          | <span data-ttu-id="97405-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="97405-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="97405-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="97405-120">Authorization</span></span> | <span data-ttu-id="97405-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97405-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97405-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97405-123">Request body</span></span>

<span data-ttu-id="97405-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97405-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97405-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="97405-125">Response</span></span>

<span data-ttu-id="97405-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97405-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97405-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="97405-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97405-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97405-129">Request</span></span>

<span data-ttu-id="97405-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97405-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97405-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="97405-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
---


### <a name="response"></a><span data-ttu-id="97405-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="97405-132">Response</span></span>

<span data-ttu-id="97405-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97405-133">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
