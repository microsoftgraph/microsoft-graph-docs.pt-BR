---
title: Criar ediscoveryCase
description: Use esta API para criar um novo ediscoveryCase.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 08383903c69b04fab82b47a623a7815e21902902
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007959"
---
# <a name="create-ediscoverycase"></a><span data-ttu-id="4635c-103">Criar ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4635c-103">Create ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4635c-104">Criar um novo objeto [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="4635c-104">Create a new [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4635c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4635c-105">Permissions</span></span>

<span data-ttu-id="4635c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4635c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4635c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4635c-108">Permission type</span></span>                        | <span data-ttu-id="4635c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4635c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4635c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4635c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4635c-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="4635c-111">User.Read</span></span>      |
| <span data-ttu-id="4635c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4635c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4635c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4635c-113">Not supported.</span></span> |
| <span data-ttu-id="4635c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4635c-114">Application</span></span>                            | <span data-ttu-id="4635c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4635c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4635c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4635c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases
```

## <a name="request-headers"></a><span data-ttu-id="4635c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4635c-117">Request headers</span></span>

| <span data-ttu-id="4635c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4635c-118">Name</span></span>          | <span data-ttu-id="4635c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4635c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4635c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4635c-120">Authorization</span></span> | <span data-ttu-id="4635c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4635c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4635c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4635c-123">Request body</span></span>

<span data-ttu-id="4635c-124">No corpo da solicitação, forneça uma representação JSON de um objeto [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="4635c-124">In the request body, supply a JSON representation of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span> <span data-ttu-id="4635c-125">A tabela a seguir lista as propriedades que podem ser enviadas com a chamada.</span><span class="sxs-lookup"><span data-stu-id="4635c-125">The following table lists properties that can be submitted with the call.</span></span>

| <span data-ttu-id="4635c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4635c-126">Property</span></span>     | <span data-ttu-id="4635c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4635c-127">Type</span></span>        | <span data-ttu-id="4635c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4635c-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4635c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4635c-129">displayName</span></span>  | <span data-ttu-id="4635c-130">string</span><span class="sxs-lookup"><span data-stu-id="4635c-130">string</span></span>      | <span data-ttu-id="4635c-131">O nome da ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4635c-131">The name of the eDiscovery case.</span></span> |

## <a name="response"></a><span data-ttu-id="4635c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4635c-132">Response</span></span>

<span data-ttu-id="4635c-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [ediscoveryCase](../resources/ediscoverycase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4635c-133">If successful, this method returns a `201 Created` response code and a new [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4635c-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4635c-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4635c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4635c-135">Request</span></span>

<span data-ttu-id="4635c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4635c-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4635c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4635c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_ediscoverycase"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-type: application/json

{
    "displayName": "My Case 1",
}
```
# <a name="c"></a>[<span data-ttu-id="4635c-138">C#</span><span class="sxs-lookup"><span data-stu-id="4635c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4635c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4635c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4635c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4635c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4635c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4635c-141">Response</span></span>

<span data-ttu-id="4635c-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4635c-142">The following is an example of the response.</span></span>

> <span data-ttu-id="4635c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4635c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases/$entity",
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


