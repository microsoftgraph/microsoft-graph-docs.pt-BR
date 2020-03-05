---
title: Remover tokenLifetimePolicy
description: Remover um tokenLifetimePolicy de um aplicativo ou servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1db08aab8d8806574cccfbdaa0e7b414d56f230d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441531"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="b607c-103">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b607c-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="b607c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b607c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b607c-105">Remover um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) de um [aplicativo](../resources/application.md) ou [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b607c-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b607c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b607c-106">Permissions</span></span>

<span data-ttu-id="b607c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b607c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b607c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b607c-109">Permission type</span></span>                        | <span data-ttu-id="b607c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b607c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b607c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b607c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b607c-112">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b607c-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b607c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b607c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b607c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b607c-114">Not supported.</span></span> |
| <span data-ttu-id="b607c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b607c-115">Application</span></span>                            | <span data-ttu-id="b607c-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b607c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b607c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b607c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="b607c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b607c-118">Request headers</span></span>

| <span data-ttu-id="b607c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b607c-119">Name</span></span>          | <span data-ttu-id="b607c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b607c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b607c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b607c-121">Authorization</span></span> | <span data-ttu-id="b607c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b607c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b607c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b607c-123">Request body</span></span>

<span data-ttu-id="b607c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b607c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b607c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b607c-125">Response</span></span>

<span data-ttu-id="b607c-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b607c-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b607c-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b607c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b607c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b607c-128">Request</span></span>

<span data-ttu-id="b607c-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b607c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="b607c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b607c-130">Response</span></span>

<span data-ttu-id="b607c-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b607c-131">The following is an example of the response.</span></span>

> <span data-ttu-id="b607c-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b607c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->