---
title: Histórico da lista
description: Obter o riskyUserHistoryItems da propriedade de navegação do histórico.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eddb74f1bc6aacc12f9a2a73df6df44b2684a5c6
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874351"
---
# <a name="list-history"></a><span data-ttu-id="581f0-103">Histórico da lista</span><span class="sxs-lookup"><span data-stu-id="581f0-103">List history</span></span>
<span data-ttu-id="581f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="581f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="581f0-105">Obter o riskyUserHistoryItems da propriedade de navegação do histórico.</span><span class="sxs-lookup"><span data-stu-id="581f0-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="581f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="581f0-106">Permissions</span></span>
<span data-ttu-id="581f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="581f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="581f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="581f0-109">Permission type</span></span>|<span data-ttu-id="581f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="581f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="581f0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="581f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="581f0-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="581f0-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="581f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="581f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="581f0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="581f0-114">Not supported.</span></span>    |
|<span data-ttu-id="581f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="581f0-115">Application</span></span> | <span data-ttu-id="581f0-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="581f0-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="581f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="581f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="581f0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="581f0-118">Optional query parameters</span></span>
<span data-ttu-id="581f0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="581f0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="581f0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="581f0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="581f0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="581f0-121">Request headers</span></span>
|<span data-ttu-id="581f0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="581f0-122">Name</span></span>|<span data-ttu-id="581f0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="581f0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="581f0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="581f0-124">Authorization</span></span>|<span data-ttu-id="581f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="581f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="581f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="581f0-127">Request body</span></span>
<span data-ttu-id="581f0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="581f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="581f0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="581f0-129">Response</span></span>

<span data-ttu-id="581f0-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção `200 OK` de [objetos riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="581f0-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="581f0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="581f0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="581f0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="581f0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="581f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="581f0-133">Response</span></span>
<span data-ttu-id="581f0-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="581f0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUserHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "5e1d812e-812e-5e1d-2e81-1d5e2e811d5e",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userId": "String",
      "initiatedBy": "String",
      "activity": {
          "riskEventTypes": [],
          "detail": "userPerformedSecuredPasswordReset"
      }
    }
  ]
}
```


