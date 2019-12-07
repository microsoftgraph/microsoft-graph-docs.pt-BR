---
title: Criar workforceIntegration
description: Criar um novo objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6da06c27296009bcf337171af6e77d5cc55eeb0
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895518"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="1a7d7-103">Criar workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="1a7d7-103">Create workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a7d7-104">Criar um novo objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="1a7d7-104">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a7d7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a7d7-105">Permissions</span></span>

<span data-ttu-id="1a7d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a7d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a7d7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a7d7-108">Permission type</span></span>                        | <span data-ttu-id="1a7d7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a7d7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a7d7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a7d7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a7d7-111">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1a7d7-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="1a7d7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a7d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a7d7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-113">Not supported.</span></span> |
| <span data-ttu-id="1a7d7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a7d7-114">Application</span></span>                            | <span data-ttu-id="1a7d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a7d7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a7d7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="1a7d7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7d7-117">Request headers</span></span>

| <span data-ttu-id="1a7d7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1a7d7-118">Name</span></span>          | <span data-ttu-id="1a7d7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a7d7-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1a7d7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a7d7-120">Authorization</span></span> | <span data-ttu-id="1a7d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a7d7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="1a7d7-123">Content-type</span></span> | <span data-ttu-id="1a7d7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a7d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7d7-126">Request body</span></span>

<span data-ttu-id="1a7d7-127">No corpo da solicitação, forneça uma representação JSON de um objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="1a7d7-127">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1a7d7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a7d7-128">Response</span></span>

<span data-ttu-id="1a7d7-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-129">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a7d7-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a7d7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a7d7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7d7-131">Request</span></span>

<span data-ttu-id="1a7d7-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="response"></a><span data-ttu-id="1a7d7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a7d7-133">Response</span></span>

<span data-ttu-id="1a7d7-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-134">The following is an example of the response.</span></span>

> <span data-ttu-id="1a7d7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a7d7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
