---
title: Histórico de lista
description: Obtenha o riskyUserHistoryItems da propriedade de navegação History.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 212f10e5794a55dec925d1ec32c37abf9708700b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897558"
---
# <a name="list-history"></a><span data-ttu-id="7fce6-103">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="7fce6-103">List history</span></span>
<span data-ttu-id="7fce6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fce6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fce6-105">Obtenha o riskyUserHistoryItems da propriedade de navegação History.</span><span class="sxs-lookup"><span data-stu-id="7fce6-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fce6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fce6-106">Permissions</span></span>
<span data-ttu-id="7fce6-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7fce6-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7fce6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7fce6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="7fce6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fce6-109">Permission type</span></span>|<span data-ttu-id="7fce6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fce6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fce6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fce6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7fce6-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fce6-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="7fce6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fce6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fce6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fce6-114">Not supported.</span></span>    |
|<span data-ttu-id="7fce6-115">Application</span><span class="sxs-lookup"><span data-stu-id="7fce6-115">Application</span></span> | <span data-ttu-id="7fce6-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fce6-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fce6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fce6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fce6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fce6-118">Optional query parameters</span></span>
<span data-ttu-id="7fce6-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fce6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7fce6-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7fce6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fce6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fce6-121">Request headers</span></span>
|<span data-ttu-id="7fce6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7fce6-122">Name</span></span>|<span data-ttu-id="7fce6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fce6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7fce6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fce6-124">Authorization</span></span>|<span data-ttu-id="7fce6-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7fce6-125">Bearer {token}.</span></span> <span data-ttu-id="7fce6-126">Required.</span><span class="sxs-lookup"><span data-stu-id="7fce6-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fce6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fce6-127">Request body</span></span>
<span data-ttu-id="7fce6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fce6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fce6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fce6-129">Response</span></span>

<span data-ttu-id="7fce6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fce6-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fce6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7fce6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fce6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fce6-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="7fce6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fce6-133">Response</span></span>
<span data-ttu-id="7fce6-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7fce6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

