---
title: Listar workforceIntegrations
description: Recupere uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8081305d23f31803691cdcb6d1c39d93080113c9
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895527"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="0e915-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="0e915-103">List workforceIntegrations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e915-104">Recupere uma lista de objetos [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="0e915-104">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e915-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e915-105">Permissions</span></span>

<span data-ttu-id="0e915-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e915-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e915-108">Permission type</span></span>                        | <span data-ttu-id="0e915-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e915-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e915-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e915-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="0e915-111">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0e915-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="0e915-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e915-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e915-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e915-113">Not supported.</span></span> |
| <span data-ttu-id="0e915-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e915-114">Application</span></span>                            | <span data-ttu-id="0e915-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e915-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e915-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e915-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e915-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e915-117">Optional query parameters</span></span>

<span data-ttu-id="0e915-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e915-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0e915-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0e915-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e915-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e915-120">Request headers</span></span>

| <span data-ttu-id="0e915-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0e915-121">Name</span></span>      |<span data-ttu-id="0e915-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e915-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e915-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e915-123">Authorization</span></span> | <span data-ttu-id="0e915-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e915-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e915-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e915-126">Request body</span></span>

<span data-ttu-id="0e915-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e915-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e915-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e915-128">Response</span></span>

<span data-ttu-id="0e915-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e915-129">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e915-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0e915-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e915-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e915-131">Request</span></span>

<span data-ttu-id="0e915-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e915-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```

### <a name="response"></a><span data-ttu-id="0e915-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e915-133">Response</span></span>

<span data-ttu-id="0e915-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e915-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0e915-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e915-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
