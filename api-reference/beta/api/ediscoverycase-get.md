---
title: Obter ediscoveryCase
description: Recupere as propriedades e os relacionamentos do objeto ediscoverycase.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9b1c8c51927139467b129b4efc0a278df5b6352d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007935"
---
# <a name="get-ediscoverycase"></a><span data-ttu-id="6c153-103">Obter ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="6c153-103">Get ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c153-104">Recupere as propriedades e os relacionamentos de um objeto [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="6c153-104">Retrieve the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c153-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c153-105">Permissions</span></span>

<span data-ttu-id="6c153-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c153-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c153-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c153-108">Permission type</span></span>                        | <span data-ttu-id="6c153-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c153-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c153-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c153-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c153-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="6c153-111">User.Read</span></span>      |
| <span data-ttu-id="6c153-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c153-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c153-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c153-113">Not supported.</span></span> |
| <span data-ttu-id="6c153-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c153-114">Application</span></span>                            | <span data-ttu-id="6c153-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c153-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c153-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c153-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c153-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c153-117">Optional query parameters</span></span>

<span data-ttu-id="6c153-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c153-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c153-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6c153-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c153-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c153-120">Request headers</span></span>

| <span data-ttu-id="6c153-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6c153-121">Name</span></span>      |<span data-ttu-id="6c153-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c153-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c153-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c153-123">Authorization</span></span> | <span data-ttu-id="6c153-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6c153-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c153-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c153-125">Request body</span></span>

<span data-ttu-id="6c153-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c153-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c153-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c153-127">Response</span></span>

<span data-ttu-id="6c153-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [ediscoveryCase](../resources/ediscoverycase.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c153-128">If successful, this method returns a `200 OK` response code and the requested [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c153-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c153-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c153-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c153-130">Request</span></span>

<span data-ttu-id="6c153-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c153-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}-->

```http
GET https://graph.microsoft.com/beta/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

### <a name="response"></a><span data-ttu-id="6c153-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c153-132">Response</span></span>

<span data-ttu-id="6c153-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c153-133">The following is an example of the response.</span></span>

> <span data-ttu-id="6c153-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c153-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
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
  "description": "Get ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

