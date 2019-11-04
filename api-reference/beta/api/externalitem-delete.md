---
title: Excluir externalItem
description: Exclua um externalItem ou externalfile.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 34eeebebb7767326e8552553a903ecd64b8e43ab
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938061"
---
# <a name="delete-externalitem"></a><span data-ttu-id="5bfd2-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="5bfd2-103">Delete externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bfd2-104">Exclua um [externalitem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="5bfd2-104">Delete an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5bfd2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bfd2-105">Permissions</span></span>

<span data-ttu-id="5bfd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bfd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bfd2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bfd2-108">Permission type</span></span>                        | <span data-ttu-id="5bfd2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bfd2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5bfd2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bfd2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bfd2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-111">Not supported.</span></span> |
| <span data-ttu-id="5bfd2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bfd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bfd2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-113">Not supported.</span></span> |
| <span data-ttu-id="5bfd2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bfd2-114">Application</span></span>                            | <span data-ttu-id="5bfd2-115">ExternalItem. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5bfd2-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bfd2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfd2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="5bfd2-117">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="5bfd2-117">Path parameters</span></span>

| <span data-ttu-id="5bfd2-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5bfd2-118">Parameter</span></span>     | <span data-ttu-id="5bfd2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bfd2-119">Type</span></span>   | <span data-ttu-id="5bfd2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bfd2-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="5bfd2-121">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="5bfd2-121">connection-id</span></span> | <span data-ttu-id="5bfd2-122">string</span><span class="sxs-lookup"><span data-stu-id="5bfd2-122">string</span></span> | <span data-ttu-id="5bfd2-123">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="5bfd2-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="5bfd2-124">item-id</span><span class="sxs-lookup"><span data-stu-id="5bfd2-124">item-id</span></span>       | <span data-ttu-id="5bfd2-125">string</span><span class="sxs-lookup"><span data-stu-id="5bfd2-125">string</span></span> | <span data-ttu-id="5bfd2-126">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="5bfd2-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5bfd2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfd2-127">Request headers</span></span>

| <span data-ttu-id="5bfd2-128">Nome</span><span class="sxs-lookup"><span data-stu-id="5bfd2-128">Name</span></span>          | <span data-ttu-id="5bfd2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bfd2-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5bfd2-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bfd2-130">Authorization</span></span> | <span data-ttu-id="5bfd2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bfd2-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfd2-133">Request body</span></span>

<span data-ttu-id="5bfd2-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bfd2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfd2-135">Response</span></span>

<span data-ttu-id="5bfd2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bfd2-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5bfd2-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5bfd2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfd2-139">Request</span></span>

<span data-ttu-id="5bfd2-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5bfd2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfd2-141">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="5bfd2-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfd2-142">The following is an example of the response.</span></span>

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
  "description": "Delete externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
