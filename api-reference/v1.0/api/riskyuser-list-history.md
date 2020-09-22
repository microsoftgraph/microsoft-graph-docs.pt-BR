---
title: Histórico de lista
description: Obtenha o riskyUserHistoryItems da propriedade de navegação History.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1fcbe019d1aa673d100cedf5904b529960cec9b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051330"
---
# <a name="list-history"></a><span data-ttu-id="7a4ba-103">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="7a4ba-103">List history</span></span>
<span data-ttu-id="7a4ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a4ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a4ba-105">Obtenha o riskyUserHistoryItems da propriedade de navegação History.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a4ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a4ba-106">Permissions</span></span>
<span data-ttu-id="7a4ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7a4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="7a4ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a4ba-109">Permission type</span></span>|<span data-ttu-id="7a4ba-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a4ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a4ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a4ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a4ba-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a4ba-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="7a4ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a4ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a4ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-114">Not supported.</span></span>    |
|<span data-ttu-id="7a4ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a4ba-115">Application</span></span> | <span data-ttu-id="7a4ba-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a4ba-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a4ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a4ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a4ba-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a4ba-118">Optional query parameters</span></span>
<span data-ttu-id="7a4ba-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7a4ba-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a4ba-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a4ba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a4ba-121">Request headers</span></span>
|<span data-ttu-id="7a4ba-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7a4ba-122">Name</span></span>|<span data-ttu-id="7a4ba-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a4ba-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a4ba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a4ba-124">Authorization</span></span>|<span data-ttu-id="7a4ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a4ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a4ba-127">Request body</span></span>
<span data-ttu-id="7a4ba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a4ba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a4ba-129">Response</span></span>

<span data-ttu-id="7a4ba-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a4ba-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a4ba-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a4ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a4ba-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="7a4ba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a4ba-133">Response</span></span>
<span data-ttu-id="7a4ba-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a4ba-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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


