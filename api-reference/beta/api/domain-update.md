---
title: Atualizar domínio
description: Atualize as propriedades do objeto de domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c221ee4ec889f77712417ca7fca1c6d7708881ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524314"
---
# <a name="update-domain"></a><span data-ttu-id="a5af2-103">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="a5af2-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5af2-104">Atualize as propriedades do objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="a5af2-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="a5af2-105">**Importante:** Somente domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a5af2-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5af2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5af2-106">Permissions</span></span>

<span data-ttu-id="a5af2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5af2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5af2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5af2-109">Permission type</span></span>      | <span data-ttu-id="a5af2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5af2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5af2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5af2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5af2-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5af2-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5af2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5af2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5af2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5af2-114">Not supported.</span></span>    |
|<span data-ttu-id="a5af2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5af2-115">Application</span></span> | <span data-ttu-id="a5af2-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5af2-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5af2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5af2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="a5af2-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="a5af2-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5af2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5af2-119">Request headers</span></span>

| <span data-ttu-id="a5af2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5af2-120">Name</span></span>       | <span data-ttu-id="a5af2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5af2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a5af2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5af2-122">Authorization</span></span>  | <span data-ttu-id="a5af2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5af2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5af2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5af2-125">Content-Type</span></span>  | <span data-ttu-id="a5af2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5af2-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5af2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5af2-127">Request body</span></span>

<span data-ttu-id="a5af2-p103">No corpo da solicitação, forneça os valores para os campos relevantes que serão atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter melhor desempenho, somente inclua valores alterados.</span><span class="sxs-lookup"><span data-stu-id="a5af2-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="a5af2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5af2-131">Response</span></span>

<span data-ttu-id="a5af2-132">Se bem-sucedido, este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5af2-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5af2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5af2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5af2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5af2-134">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="a5af2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5af2-135">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/domain-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
