---
title: Criar workforceIntegration
description: Criar um novo objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b818b55d95485ca17aff581f8b986f3fbb01465d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451270"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="94dd0-103">Criar workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="94dd0-103">Create workforceIntegration</span></span>

<span data-ttu-id="94dd0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94dd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94dd0-105">Criar um novo objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="94dd0-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94dd0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94dd0-106">Permissions</span></span>

<span data-ttu-id="94dd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94dd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94dd0-109">Permission type</span></span>                        | <span data-ttu-id="94dd0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94dd0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94dd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94dd0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94dd0-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="94dd0-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="94dd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94dd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94dd0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94dd0-114">Not supported.</span></span> |
| <span data-ttu-id="94dd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94dd0-115">Application</span></span>                            | <span data-ttu-id="94dd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94dd0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94dd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94dd0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="94dd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94dd0-118">Request headers</span></span>

| <span data-ttu-id="94dd0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="94dd0-119">Name</span></span>          | <span data-ttu-id="94dd0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="94dd0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="94dd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="94dd0-121">Authorization</span></span> | <span data-ttu-id="94dd0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94dd0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94dd0-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="94dd0-124">Content-type</span></span> | <span data-ttu-id="94dd0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94dd0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94dd0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94dd0-127">Request body</span></span>

<span data-ttu-id="94dd0-128">No corpo da solicitação, forneça uma representação JSON de um objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="94dd0-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94dd0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94dd0-129">Response</span></span>

<span data-ttu-id="94dd0-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94dd0-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94dd0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94dd0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94dd0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94dd0-132">Request</span></span>

<span data-ttu-id="94dd0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94dd0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94dd0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94dd0-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="94dd0-135">C#</span><span class="sxs-lookup"><span data-stu-id="94dd0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94dd0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94dd0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94dd0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94dd0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94dd0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94dd0-138">Response</span></span>

<span data-ttu-id="94dd0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94dd0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="94dd0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94dd0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
