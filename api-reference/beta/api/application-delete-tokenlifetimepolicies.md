---
title: Remover tokenLifetimePolicy
description: Remover um tokenLifetimePolicy de um aplicativo ou servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 055da6eb449c8600e39755f4725ce72af35af045
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234061"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="30a3b-103">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="30a3b-103">Remove tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a3b-104">Remover um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) de um [aplicativo](../resources/application.md) ou [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="30a3b-104">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="30a3b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30a3b-105">Permissions</span></span>

<span data-ttu-id="30a3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30a3b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30a3b-108">Permission type</span></span>                        | <span data-ttu-id="30a3b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30a3b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="30a3b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30a3b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="30a3b-111">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="30a3b-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="30a3b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30a3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30a3b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30a3b-113">Not supported.</span></span> |
| <span data-ttu-id="30a3b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30a3b-114">Application</span></span>                            | <span data-ttu-id="30a3b-115">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="30a3b-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30a3b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30a3b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="30a3b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30a3b-117">Request headers</span></span>

| <span data-ttu-id="30a3b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="30a3b-118">Name</span></span>          | <span data-ttu-id="30a3b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="30a3b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="30a3b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="30a3b-120">Authorization</span></span> | <span data-ttu-id="30a3b-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="30a3b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="30a3b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30a3b-122">Request body</span></span>

<span data-ttu-id="30a3b-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30a3b-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30a3b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a3b-124">Response</span></span>

<span data-ttu-id="30a3b-125">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="30a3b-125">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="30a3b-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30a3b-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30a3b-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30a3b-127">Request</span></span>

<span data-ttu-id="30a3b-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="30a3b-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="30a3b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a3b-129">Response</span></span>

<span data-ttu-id="30a3b-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="30a3b-130">The following is an example of the response.</span></span>

> <span data-ttu-id="30a3b-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30a3b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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