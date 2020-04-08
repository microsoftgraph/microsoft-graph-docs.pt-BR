---
title: Excluir certificateBasedAuthConfiguration
description: Exclua certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f549c29015f5352fc9674ecd0a0c1a1422b125d3
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181060"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="ada3c-103">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada3c-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="ada3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ada3c-105">Excluir um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ada3c-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ada3c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ada3c-106">Permissions</span></span>

<span data-ttu-id="ada3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ada3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ada3c-109">Permission type</span></span>                        | <span data-ttu-id="ada3c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ada3c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ada3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ada3c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ada3c-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada3c-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="ada3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ada3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ada3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ada3c-114">Not supported.</span></span> |
| <span data-ttu-id="ada3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ada3c-115">Application</span></span>    | <span data-ttu-id="ada3c-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada3c-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ada3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ada3c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ada3c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ada3c-118">Request headers</span></span>

| <span data-ttu-id="ada3c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ada3c-119">Name</span></span>          | <span data-ttu-id="ada3c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ada3c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ada3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ada3c-121">Authorization</span></span> | <span data-ttu-id="ada3c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ada3c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ada3c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ada3c-123">Request body</span></span>

<span data-ttu-id="ada3c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ada3c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ada3c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ada3c-125">Response</span></span>

<span data-ttu-id="ada3c-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ada3c-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ada3c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ada3c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ada3c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ada3c-129">Request</span></span>

<span data-ttu-id="ada3c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ada3c-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ada3c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ada3c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="ada3c-132">C#</span><span class="sxs-lookup"><span data-stu-id="ada3c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ada3c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ada3c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ada3c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ada3c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ada3c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ada3c-135">Response</span></span>

<span data-ttu-id="ada3c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ada3c-136">The following is an example of the response.</span></span>

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
