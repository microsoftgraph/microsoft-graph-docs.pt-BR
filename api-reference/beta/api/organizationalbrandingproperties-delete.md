---
title: Excluir organizationalBrandingProperties
description: Exclua organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c698becef5cb0ca7950ba9c210356aa76ee1814
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031911"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="81093-103">Excluir organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="81093-103">Delete organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81093-104">Excluir um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="81093-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81093-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="81093-105">Permissions</span></span>

<span data-ttu-id="81093-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81093-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81093-108">Permission type</span></span>                        | <span data-ttu-id="81093-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81093-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81093-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81093-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81093-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81093-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="81093-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81093-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81093-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81093-113">Not supported.</span></span> |
| <span data-ttu-id="81093-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81093-114">Application</span></span>                            | <span data-ttu-id="81093-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81093-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81093-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81093-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="81093-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81093-117">Request headers</span></span>

| <span data-ttu-id="81093-118">Nome</span><span class="sxs-lookup"><span data-stu-id="81093-118">Name</span></span>          | <span data-ttu-id="81093-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="81093-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81093-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="81093-120">Authorization</span></span> | <span data-ttu-id="81093-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81093-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81093-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81093-123">Request body</span></span>

<span data-ttu-id="81093-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81093-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81093-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="81093-125">Response</span></span>

<span data-ttu-id="81093-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81093-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81093-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81093-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81093-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81093-129">Request</span></span>

<span data-ttu-id="81093-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81093-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

### <a name="response"></a><span data-ttu-id="81093-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="81093-131">Response</span></span>

<span data-ttu-id="81093-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81093-132">The following is an example of the response.</span></span>

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
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->