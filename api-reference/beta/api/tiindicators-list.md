---
title: Listar indicadores de inteligência de ameaças
description: Recupere uma lista de objetos tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4e4aa089614548379dc23e92bec5fff50696fc5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987912"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="d4240-103">Listar indicadores de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="d4240-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4240-104">Recupere uma lista de objetos [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="d4240-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4240-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4240-105">Permissions</span></span>

<span data-ttu-id="d4240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4240-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4240-108">Permission type</span></span>     | <span data-ttu-id="d4240-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4240-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4240-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4240-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4240-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d4240-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="d4240-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4240-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4240-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4240-113">Not supported.</span></span> |
| <span data-ttu-id="d4240-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4240-114">Application</span></span>                            | <span data-ttu-id="d4240-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d4240-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4240-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4240-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4240-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4240-117">Optional query parameters</span></span>

<span data-ttu-id="d4240-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4240-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d4240-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d4240-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4240-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4240-120">Request headers</span></span>

| <span data-ttu-id="d4240-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d4240-121">Name</span></span>      |<span data-ttu-id="d4240-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4240-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4240-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4240-123">Authorization</span></span> | <span data-ttu-id="d4240-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d4240-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4240-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4240-125">Request body</span></span>

<span data-ttu-id="d4240-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4240-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4240-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4240-127">Response</span></span>

<span data-ttu-id="d4240-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4240-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4240-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4240-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4240-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4240-130">Request</span></span>

<span data-ttu-id="d4240-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4240-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4240-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4240-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4240-133">C#</span><span class="sxs-lookup"><span data-stu-id="d4240-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4240-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4240-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4240-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d4240-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d4240-136">Java</span><span class="sxs-lookup"><span data-stu-id="d4240-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4240-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4240-137">Response</span></span>

<span data-ttu-id="d4240-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4240-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d4240-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4240-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d4240-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4240-140">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
