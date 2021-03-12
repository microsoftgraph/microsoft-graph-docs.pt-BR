---
title: Excluir organizationalBrandingProperties
description: Excluir organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4faef793d2ab02eb530ee839fdd683de04f4a179
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722510"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="37745-103">Excluir organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="37745-103">Delete organizationalBrandingProperties</span></span>

<span data-ttu-id="37745-104">[Exclua um objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="37745-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37745-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="37745-105">Permissions</span></span>

<span data-ttu-id="37745-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37745-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37745-108">Permission type</span></span>                        | <span data-ttu-id="37745-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37745-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37745-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37745-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="37745-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37745-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="37745-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37745-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37745-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37745-113">Not supported.</span></span> |
| <span data-ttu-id="37745-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37745-114">Application</span></span>                            | <span data-ttu-id="37745-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37745-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37745-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37745-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="37745-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37745-117">Request headers</span></span>

| <span data-ttu-id="37745-118">Nome</span><span class="sxs-lookup"><span data-stu-id="37745-118">Name</span></span>          | <span data-ttu-id="37745-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="37745-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="37745-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="37745-120">Authorization</span></span> | <span data-ttu-id="37745-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37745-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37745-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37745-123">Request body</span></span>

<span data-ttu-id="37745-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37745-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37745-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="37745-125">Response</span></span>

<span data-ttu-id="37745-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37745-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37745-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37745-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37745-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37745-129">Request</span></span>

<span data-ttu-id="37745-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37745-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

### <a name="response"></a><span data-ttu-id="37745-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="37745-131">Response</span></span>

<span data-ttu-id="37745-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37745-132">The following is an example of the response.</span></span>

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
