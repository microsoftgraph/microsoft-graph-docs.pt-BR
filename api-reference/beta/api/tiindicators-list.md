---
title: Listar indicadores de inteligência de ameaças
description: Recupere uma lista de objetos tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 98f058d94c101a2f664f21ea05252a51476b426d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330628"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="e14ae-103">Listar indicadores de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="e14ae-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e14ae-104">Recupere uma lista de objetos [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="e14ae-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e14ae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e14ae-105">Permissions</span></span>

<span data-ttu-id="e14ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e14ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e14ae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e14ae-108">Permission type</span></span>     | <span data-ttu-id="e14ae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e14ae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e14ae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e14ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e14ae-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e14ae-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="e14ae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e14ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e14ae-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e14ae-113">Not supported.</span></span> |
| <span data-ttu-id="e14ae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e14ae-114">Application</span></span>                            | <span data-ttu-id="e14ae-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e14ae-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e14ae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e14ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e14ae-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e14ae-117">Optional query parameters</span></span>

<span data-ttu-id="e14ae-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e14ae-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e14ae-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e14ae-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e14ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e14ae-120">Request headers</span></span>

| <span data-ttu-id="e14ae-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e14ae-121">Name</span></span>      |<span data-ttu-id="e14ae-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e14ae-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e14ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e14ae-123">Authorization</span></span> | <span data-ttu-id="e14ae-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e14ae-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e14ae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e14ae-125">Request body</span></span>

<span data-ttu-id="e14ae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e14ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e14ae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e14ae-127">Response</span></span>

<span data-ttu-id="e14ae-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e14ae-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e14ae-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e14ae-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e14ae-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e14ae-130">Request</span></span>

<span data-ttu-id="e14ae-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e14ae-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```

### <a name="response"></a><span data-ttu-id="e14ae-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e14ae-132">Response</span></span>

<span data-ttu-id="e14ae-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e14ae-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e14ae-134">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e14ae-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e14ae-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e14ae-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "action": "action-value",
      "activityGroupNames": [
        "activityGroupNames-value"
      ],
      "additionalInformation": "additionalInformation-value",
      "azureTenantId": "azureTenantId-value",
      "confidence": 99,
      "description": "description-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
