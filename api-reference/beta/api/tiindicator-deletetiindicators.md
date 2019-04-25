---
title: 'tiIndicator: deleteTiIndicators'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 49475f15520f02cc36bb1bf37af9a5849a8ee245
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544655"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="d989f-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="d989f-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d989f-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="d989f-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="d989f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d989f-105">Permissions</span></span>

<span data-ttu-id="d989f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d989f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d989f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d989f-108">Permission type</span></span> | <span data-ttu-id="d989f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d989f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d989f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d989f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d989f-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d989f-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="d989f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d989f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d989f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d989f-113">Not supported.</span></span> |
| <span data-ttu-id="d989f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d989f-114">Application</span></span>                            | <span data-ttu-id="d989f-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d989f-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="d989f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d989f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="d989f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d989f-117">Request headers</span></span>

| <span data-ttu-id="d989f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d989f-118">Name</span></span>          | <span data-ttu-id="d989f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d989f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d989f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d989f-120">Authorization</span></span> | <span data-ttu-id="d989f-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d989f-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d989f-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d989f-122">Request body</span></span>

<span data-ttu-id="d989f-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d989f-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d989f-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d989f-124">Parameter</span></span>    | <span data-ttu-id="d989f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d989f-125">Type</span></span>        | <span data-ttu-id="d989f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d989f-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d989f-127">valor</span><span class="sxs-lookup"><span data-stu-id="d989f-127">value</span></span>|<span data-ttu-id="d989f-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d989f-128">String collection</span></span>| <span data-ttu-id="d989f-129">Coleção de tiIndicator `id`s a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="d989f-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="d989f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d989f-130">Response</span></span>

<span data-ttu-id="d989f-131">Se bem-sucedido, este método retorna `200, OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d989f-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d989f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d989f-132">Examples</span></span>

<span data-ttu-id="d989f-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d989f-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d989f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d989f-134">Request</span></span>

<span data-ttu-id="d989f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d989f-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d989f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d989f-136">Response</span></span>

<span data-ttu-id="d989f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d989f-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d989f-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d989f-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d989f-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d989f-139">All the properties will be returned from an actual call.</span></span>

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
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
