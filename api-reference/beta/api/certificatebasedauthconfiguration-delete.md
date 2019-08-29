---
title: Excluir certificateBasedAuthConfiguration
description: Exclua certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c9fc5a1bcc524551fd83efe54ab5dabf9bfc943
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667608"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="85ae4-103">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="85ae4-103">Delete certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85ae4-104">Excluir um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="85ae4-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85ae4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85ae4-105">Permissions</span></span>

<span data-ttu-id="85ae4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85ae4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85ae4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85ae4-108">Permission type</span></span>                        | <span data-ttu-id="85ae4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85ae4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85ae4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85ae4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85ae4-111">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85ae4-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="85ae4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85ae4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85ae4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85ae4-113">Not supported.</span></span> |
| <span data-ttu-id="85ae4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85ae4-114">Application</span></span>    | <span data-ttu-id="85ae4-115">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85ae4-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85ae4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85ae4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85ae4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85ae4-117">Request headers</span></span>

| <span data-ttu-id="85ae4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="85ae4-118">Name</span></span>          | <span data-ttu-id="85ae4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="85ae4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85ae4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="85ae4-120">Authorization</span></span> | <span data-ttu-id="85ae4-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="85ae4-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="85ae4-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85ae4-122">Request body</span></span>

<span data-ttu-id="85ae4-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85ae4-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85ae4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="85ae4-124">Response</span></span>

<span data-ttu-id="85ae4-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85ae4-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85ae4-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85ae4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85ae4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85ae4-128">Request</span></span>

<span data-ttu-id="85ae4-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85ae4-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```

### <a name="response"></a><span data-ttu-id="85ae4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="85ae4-130">Response</span></span>

<span data-ttu-id="85ae4-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85ae4-131">The following is an example of the response.</span></span>

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
