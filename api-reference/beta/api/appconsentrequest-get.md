---
title: Obter appConsentRequest
description: Leia as propriedades e as relações de um objeto appConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 766bf7cd58630a74d8f0ac2d0c0982ca87b1d4f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952177"
---
# <a name="get-appconsentrequest"></a><span data-ttu-id="22732-103">Obter appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="22732-103">Get appConsentRequest</span></span>
<span data-ttu-id="22732-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22732-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22732-105">Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="22732-105">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22732-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22732-106">Permissions</span></span>
<span data-ttu-id="22732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22732-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22732-109">Permission type</span></span>|<span data-ttu-id="22732-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22732-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22732-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22732-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22732-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22732-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="22732-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22732-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22732-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22732-114">Not supported.</span></span>|
|<span data-ttu-id="22732-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22732-115">Application</span></span>|<span data-ttu-id="22732-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22732-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22732-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22732-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22732-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22732-118">Optional query parameters</span></span>
<span data-ttu-id="22732-119">Este método dá suporte ao  `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22732-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="22732-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="22732-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22732-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22732-121">Request headers</span></span>
|<span data-ttu-id="22732-122">Nome</span><span class="sxs-lookup"><span data-stu-id="22732-122">Name</span></span>|<span data-ttu-id="22732-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="22732-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22732-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="22732-124">Authorization</span></span>|<span data-ttu-id="22732-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22732-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22732-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22732-127">Request body</span></span>
<span data-ttu-id="22732-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22732-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22732-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="22732-129">Response</span></span>

<span data-ttu-id="22732-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22732-130">If successful, this method returns a `200 OK` response code and an [appConsentRequest](../resources/appconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22732-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22732-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22732-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22732-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed
```


### <a name="response"></a><span data-ttu-id="22732-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="22732-133">Response</span></span>
<span data-ttu-id="22732-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22732-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests/$entity",
  "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
  "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
  "appDisplayName": "Moodle",
  "consentType": "Dynamic",
  "pendingScopes": [],
  "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
  "userConsentRequests": []
}
```

