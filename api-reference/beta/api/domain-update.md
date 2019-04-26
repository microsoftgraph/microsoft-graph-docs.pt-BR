---
title: Atualizar domínio
description: Atualize as propriedades do objeto Domain.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 36bf901ff9e5c0ca9e8164aebac8559ad78d2eef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326243"
---
# <a name="update-domain"></a><span data-ttu-id="11696-103">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="11696-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11696-104">Atualize as propriedades do objeto Domain.</span><span class="sxs-lookup"><span data-stu-id="11696-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="11696-105">**Importante:** Somente os domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="11696-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="11696-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11696-106">Permissions</span></span>

<span data-ttu-id="11696-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="11696-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11696-109">Permission type</span></span>      | <span data-ttu-id="11696-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11696-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11696-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11696-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11696-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11696-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11696-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11696-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11696-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11696-114">Not supported.</span></span>    |
|<span data-ttu-id="11696-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11696-115">Application</span></span> | <span data-ttu-id="11696-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11696-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11696-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11696-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="11696-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="11696-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11696-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11696-119">Request headers</span></span>

| <span data-ttu-id="11696-120">Nome</span><span class="sxs-lookup"><span data-stu-id="11696-120">Name</span></span>       | <span data-ttu-id="11696-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="11696-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="11696-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11696-122">Authorization</span></span>  | <span data-ttu-id="11696-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11696-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11696-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11696-125">Content-Type</span></span>  | <span data-ttu-id="11696-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11696-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="11696-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11696-127">Request body</span></span>

<span data-ttu-id="11696-128">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="11696-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="11696-129">As propriedades existentes não incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="11696-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="11696-130">Para obter o melhor desempenho, inclua somente valores alterados.</span><span class="sxs-lookup"><span data-stu-id="11696-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="11696-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="11696-131">Response</span></span>

<span data-ttu-id="11696-132">Se tiver êxito, este método retornará `204 No Content` um código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11696-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="11696-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11696-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11696-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11696-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="11696-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="11696-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
