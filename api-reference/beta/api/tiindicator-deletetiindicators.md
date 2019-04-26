---
title: 'tiIndicator: deleteTiIndicators'
description: Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d5ceaa7e7c0402719b8ee202053da54ad235cc28
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335292"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="f45a6-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="f45a6-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f45a6-104">Excluir vários indicadores de inteligência de ameaça (TI) em uma solicitação em vez de várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="f45a6-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="f45a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f45a6-105">Permissions</span></span>

<span data-ttu-id="f45a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f45a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f45a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f45a6-108">Permission type</span></span> | <span data-ttu-id="f45a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f45a6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f45a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f45a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f45a6-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f45a6-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="f45a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f45a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f45a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f45a6-113">Not supported.</span></span> |
| <span data-ttu-id="f45a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f45a6-114">Application</span></span>                            | <span data-ttu-id="f45a6-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f45a6-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="f45a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f45a6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="f45a6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f45a6-117">Request headers</span></span>

| <span data-ttu-id="f45a6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f45a6-118">Name</span></span>          | <span data-ttu-id="f45a6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f45a6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f45a6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f45a6-120">Authorization</span></span> | <span data-ttu-id="f45a6-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f45a6-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f45a6-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f45a6-122">Request body</span></span>

<span data-ttu-id="f45a6-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f45a6-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f45a6-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f45a6-124">Parameter</span></span>    | <span data-ttu-id="f45a6-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f45a6-125">Type</span></span>        | <span data-ttu-id="f45a6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f45a6-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f45a6-127">valor</span><span class="sxs-lookup"><span data-stu-id="f45a6-127">value</span></span>|<span data-ttu-id="f45a6-128">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f45a6-128">String collection</span></span>| <span data-ttu-id="f45a6-129">Coleção de tiIndicator `id`s a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="f45a6-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="f45a6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f45a6-130">Response</span></span>

<span data-ttu-id="f45a6-131">Se bem-sucedido, este método retorna `200, OK` o código de resposta e um objeto da coleção [resultInfo](../resources/resultinfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f45a6-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f45a6-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f45a6-132">Examples</span></span>

<span data-ttu-id="f45a6-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f45a6-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f45a6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f45a6-134">Request</span></span>

<span data-ttu-id="f45a6-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f45a6-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f45a6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f45a6-136">Response</span></span>

<span data-ttu-id="f45a6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f45a6-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f45a6-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f45a6-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f45a6-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f45a6-139">All the properties will be returned from an actual call.</span></span>

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
