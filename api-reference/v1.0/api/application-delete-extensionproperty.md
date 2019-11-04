---
title: Delete extensionproperty
description: Excluir uma extensãoproperty.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30d45906695e2e9bfb256f5dedf4a2108308b63d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939744"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="6806d-103">Delete extensionproperty</span><span class="sxs-lookup"><span data-stu-id="6806d-103">Delete extensionProperty</span></span>

<span data-ttu-id="6806d-104">Excluir uma [extensãoproperty](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="6806d-104">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6806d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6806d-105">Permissions</span></span>

<span data-ttu-id="6806d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6806d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6806d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6806d-108">Permission type</span></span>      | <span data-ttu-id="6806d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6806d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6806d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6806d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6806d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6806d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6806d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6806d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6806d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6806d-113">Not supported.</span></span>    |
|<span data-ttu-id="6806d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6806d-114">Application</span></span> | <span data-ttu-id="6806d-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6806d-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6806d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6806d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6806d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6806d-117">Request headers</span></span>

| <span data-ttu-id="6806d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6806d-118">Name</span></span>       | <span data-ttu-id="6806d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6806d-119">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="6806d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6806d-120">Authorization</span></span>  | <span data-ttu-id="6806d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6806d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6806d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6806d-123">Request body</span></span>

<span data-ttu-id="6806d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6806d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6806d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6806d-125">Response</span></span>

<span data-ttu-id="6806d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6806d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6806d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6806d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6806d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6806d-129">Request</span></span>

<span data-ttu-id="6806d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6806d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```

### <a name="response"></a><span data-ttu-id="6806d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6806d-131">Response</span></span>

<span data-ttu-id="6806d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6806d-132">The following is an example of the response.</span></span>

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
  "description": "Delete extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
