---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação, em vez de várias solicitações, e a solicitação contém IDs externas em vez de IDs.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 82cdd0d9688e778982244a06a2a2e5d558d25807
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537032"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="1c300-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="1c300-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c300-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação, em vez de várias solicitações, quando a solicitação contém IDs externas em vez de IDs.</span><span class="sxs-lookup"><span data-stu-id="1c300-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c300-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c300-105">Permissions</span></span>

<span data-ttu-id="1c300-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c300-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c300-108">Permission type</span></span>  | <span data-ttu-id="1c300-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c300-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c300-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c300-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c300-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1c300-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="1c300-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c300-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c300-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c300-113">Not supported.</span></span> |
| <span data-ttu-id="1c300-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c300-114">Application</span></span>                            | <span data-ttu-id="1c300-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1c300-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c300-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c300-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="1c300-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c300-117">Request headers</span></span>

| <span data-ttu-id="1c300-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1c300-118">Name</span></span>          | <span data-ttu-id="1c300-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c300-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1c300-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c300-120">Authorization</span></span> | <span data-ttu-id="1c300-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1c300-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c300-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c300-122">Request body</span></span>

<span data-ttu-id="1c300-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c300-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c300-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1c300-124">Parameter</span></span>    | <span data-ttu-id="1c300-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c300-125">Type</span></span>        | <span data-ttu-id="1c300-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c300-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c300-127">valor</span><span class="sxs-lookup"><span data-stu-id="1c300-127">value</span></span>|<span data-ttu-id="1c300-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c300-128">String collection</span></span>| <span data-ttu-id="1c300-129">Coleção de `externalIds` objetos **tiIndicator** a serem excluídos.</span><span class="sxs-lookup"><span data-stu-id="1c300-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="1c300-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c300-130">Response</span></span>

<span data-ttu-id="1c300-131">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c300-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c300-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c300-132">Examples</span></span>

<span data-ttu-id="1c300-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1c300-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1c300-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c300-134">Request</span></span>

<span data-ttu-id="1c300-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c300-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1c300-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c300-136">Response</span></span>

<span data-ttu-id="1c300-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c300-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1c300-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c300-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c300-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c300-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
