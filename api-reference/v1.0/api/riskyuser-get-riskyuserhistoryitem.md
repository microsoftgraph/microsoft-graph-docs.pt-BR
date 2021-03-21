---
title: Obter histórico
description: Leia as propriedades e as relações de um objeto riskyUserHistoryItem.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f3af631bc0c49d6b0ea2a71325df2b559917a2e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959519"
---
# <a name="get-history"></a><span data-ttu-id="5697f-103">Obter histórico</span><span class="sxs-lookup"><span data-stu-id="5697f-103">Get history</span></span>
<span data-ttu-id="5697f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5697f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5697f-105">Leia as propriedades e as relações de um [objeto riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5697f-105">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>


><span data-ttu-id="5697f-106">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5697f-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5697f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5697f-107">Permissions</span></span>
<span data-ttu-id="5697f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5697f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="5697f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5697f-110">Permission type</span></span>      | <span data-ttu-id="5697f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5697f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5697f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5697f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5697f-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5697f-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="5697f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5697f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5697f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5697f-115">Not supported.</span></span>    |
|<span data-ttu-id="5697f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5697f-116">Application</span></span> | <span data-ttu-id="5697f-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5697f-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5697f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5697f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{userId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5697f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5697f-119">Optional query parameters</span></span>
<span data-ttu-id="5697f-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5697f-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5697f-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5697f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5697f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5697f-122">Request headers</span></span>
|<span data-ttu-id="5697f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5697f-123">Name</span></span>|<span data-ttu-id="5697f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5697f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5697f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5697f-125">Authorization</span></span>|<span data-ttu-id="5697f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5697f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5697f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5697f-128">Request body</span></span>
<span data-ttu-id="5697f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5697f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5697f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5697f-130">Response</span></span>

<span data-ttu-id="5697f-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5697f-131">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5697f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5697f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5697f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5697f-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```


### <a name="response"></a><span data-ttu-id="5697f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5697f-134">Response</span></span>
<span data-ttu-id="5697f-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5697f-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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


