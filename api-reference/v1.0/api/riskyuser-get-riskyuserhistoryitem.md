---
title: Obter histórico
description: Leia as propriedades e os relacionamentos de um objeto riskyUserHistoryItem.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 141aaa6a1c0642159cccfe075aa8934fa65883cd
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897572"
---
# <a name="get-history"></a><span data-ttu-id="73b5a-103">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="73b5a-103">Get history</span></span>
<span data-ttu-id="73b5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73b5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73b5a-105">Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="73b5a-105">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>


><span data-ttu-id="73b5a-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="73b5a-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="73b5a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="73b5a-107">Permissions</span></span>
<span data-ttu-id="73b5a-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="73b5a-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="73b5a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="73b5a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="73b5a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73b5a-110">Permission type</span></span>      | <span data-ttu-id="73b5a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73b5a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b5a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73b5a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73b5a-113">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="73b5a-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="73b5a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73b5a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73b5a-115">Not supported.</span></span>    |
|<span data-ttu-id="73b5a-116">Application</span><span class="sxs-lookup"><span data-stu-id="73b5a-116">Application</span></span> | <span data-ttu-id="73b5a-117">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="73b5a-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b5a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73b5a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{userId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73b5a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73b5a-119">Optional query parameters</span></span>
<span data-ttu-id="73b5a-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73b5a-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="73b5a-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="73b5a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="73b5a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73b5a-122">Request headers</span></span>
|<span data-ttu-id="73b5a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="73b5a-123">Name</span></span>|<span data-ttu-id="73b5a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="73b5a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73b5a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="73b5a-125">Authorization</span></span>|<span data-ttu-id="73b5a-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="73b5a-126">Bearer {token}.</span></span> <span data-ttu-id="73b5a-127">Required.</span><span class="sxs-lookup"><span data-stu-id="73b5a-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73b5a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73b5a-128">Request body</span></span>
<span data-ttu-id="73b5a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73b5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b5a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="73b5a-130">Response</span></span>

<span data-ttu-id="73b5a-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73b5a-131">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73b5a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73b5a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73b5a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73b5a-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```


### <a name="response"></a><span data-ttu-id="73b5a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="73b5a-134">Response</span></span>
<span data-ttu-id="73b5a-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="73b5a-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": 
  {
    "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
      "@odata.type": "microsoft.graph.riskUserActivity"
    }
  }
}
```

