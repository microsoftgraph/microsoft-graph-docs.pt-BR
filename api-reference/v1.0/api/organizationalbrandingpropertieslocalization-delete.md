---
title: Excluir organizacional localizadaBrandingProperties
description: Exclua organizationalBrandingProperties para uma localização específica.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d15d5e5ef20cc7d18fbd26097fcdc19f7802ca0f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722504"
---
# <a name="delete-localized-organizationalbrandingproperties"></a><span data-ttu-id="72dd5-103">Excluir organizacional localizadaBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="72dd5-103">Delete Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="72dd5-104">[Exclua um objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="72dd5-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72dd5-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="72dd5-105">Permissions</span></span>

<span data-ttu-id="72dd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72dd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72dd5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72dd5-108">Permission type</span></span>                        | <span data-ttu-id="72dd5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72dd5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72dd5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72dd5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="72dd5-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72dd5-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="72dd5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72dd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72dd5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72dd5-113">Not supported.</span></span> |
| <span data-ttu-id="72dd5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72dd5-114">Application</span></span>                            | <span data-ttu-id="72dd5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72dd5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72dd5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72dd5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="72dd5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72dd5-117">Request headers</span></span>

| <span data-ttu-id="72dd5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="72dd5-118">Name</span></span>          | <span data-ttu-id="72dd5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="72dd5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="72dd5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="72dd5-120">Authorization</span></span> | <span data-ttu-id="72dd5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72dd5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72dd5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72dd5-123">Request body</span></span>

<span data-ttu-id="72dd5-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72dd5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72dd5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="72dd5-125">Response</span></span>

<span data-ttu-id="72dd5-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72dd5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72dd5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72dd5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72dd5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72dd5-129">Request</span></span>

<span data-ttu-id="72dd5-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72dd5-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

### <a name="response"></a><span data-ttu-id="72dd5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="72dd5-131">Response</span></span>

<span data-ttu-id="72dd5-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72dd5-132">The following is an example of the response.</span></span>

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
