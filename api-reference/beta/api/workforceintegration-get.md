---
title: Obter workforceIntegration
description: Recupere as propriedades e os relacionamentos do objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2738959b356faba1d6d27ae48fa94dcf6f28dbe9
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895523"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="b0d5a-103">Obter workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b0d5a-103">Get workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0d5a-104">Recupere as propriedades e os relacionamentos do objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0d5a-104">Retrieve the properties and relationships of [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0d5a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0d5a-105">Permissions</span></span>

<span data-ttu-id="b0d5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0d5a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0d5a-108">Permission type</span></span>                        | <span data-ttu-id="b0d5a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0d5a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0d5a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0d5a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0d5a-111">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b0d5a-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="b0d5a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0d5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0d5a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-113">Not supported.</span></span> |
| <span data-ttu-id="b0d5a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0d5a-114">Application</span></span>                            | <span data-ttu-id="b0d5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0d5a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d5a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0d5a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0d5a-117">Optional query parameters</span></span>

<span data-ttu-id="b0d5a-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b0d5a-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b0d5a-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0d5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d5a-120">Request headers</span></span>

| <span data-ttu-id="b0d5a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b0d5a-121">Name</span></span>      |<span data-ttu-id="b0d5a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0d5a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0d5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0d5a-123">Authorization</span></span> | <span data-ttu-id="b0d5a-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b0d5a-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0d5a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d5a-125">Request body</span></span>

<span data-ttu-id="b0d5a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0d5a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0d5a-127">Response</span></span>

<span data-ttu-id="b0d5a-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workforceIntegration](../resources/workforceintegration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-128">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0d5a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b0d5a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0d5a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d5a-130">Request</span></span>

<span data-ttu-id="b0d5a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```

### <a name="response"></a><span data-ttu-id="b0d5a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0d5a-132">Response</span></span>

<span data-ttu-id="b0d5a-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-133">The following is an example of the response.</span></span>

> <span data-ttu-id="b0d5a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0d5a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supports": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->