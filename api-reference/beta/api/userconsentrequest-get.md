---
title: Obter userConsentRequest
description: Leia as propriedades e as relações de um objeto userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8a3a7b1f086462210d77d2ab2f7b61ec116a38c7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965008"
---
# <a name="get-userconsentrequest"></a><span data-ttu-id="269e7-103">Obter userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="269e7-103">Get userConsentRequest</span></span>
<span data-ttu-id="269e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="269e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="269e7-105">Leia as propriedades e as relações de um [objeto userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="269e7-105">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="269e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="269e7-106">Permissions</span></span>
<span data-ttu-id="269e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="269e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="269e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="269e7-109">Permission type</span></span>|<span data-ttu-id="269e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="269e7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="269e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="269e7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="269e7-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="269e7-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="269e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="269e7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="269e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="269e7-114">Not supported.</span></span>|
|<span data-ttu-id="269e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="269e7-115">Application</span></span>|<span data-ttu-id="269e7-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="269e7-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="269e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="269e7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{appconsentrequest-id}/userConsentRequests/{userconsentrequest-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="269e7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="269e7-118">Optional query parameters</span></span>
<span data-ttu-id="269e7-119">Este método dá suporte ao  `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="269e7-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="269e7-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="269e7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="269e7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="269e7-121">Request headers</span></span>
|<span data-ttu-id="269e7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="269e7-122">Name</span></span>|<span data-ttu-id="269e7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="269e7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="269e7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="269e7-124">Authorization</span></span>|<span data-ttu-id="269e7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="269e7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="269e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="269e7-127">Request body</span></span>
<span data-ttu-id="269e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="269e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="269e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="269e7-129">Response</span></span>

<span data-ttu-id="269e7-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userConsentRequest](../resources/userconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="269e7-130">If successful, this method returns a `200 OK` response code and a [userConsentRequest](../resources/userconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="269e7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="269e7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="269e7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="269e7-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/acef2660-d194-4943-b927-4fe4fb5cb7e3
```


### <a name="response"></a><span data-ttu-id="269e7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="269e7-133">Response</span></span>
<span data-ttu-id="269e7-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="269e7-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests/$entity",
  "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
  "reason": "I need access",
  "status": "Completed",
  "createdDateTime": "2019-10-18T19:07:19.7374554Z",
  "createdBy": {
    "user": {
      "id": "db60ab61-caea-4889-a824-98de31ef31b5",
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "mail": "AlexW@contoso.com"
    }
  },
  "approval@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
  "approval": {
    "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
    "steps@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/steps",
    "steps": [
      {
        "id": "f5a4ca4a-1316-4872-8112-993c55dab51e",
        "displayName": null,
        "reviewedDateTime": "2019-10-19T04:12:09.633Z",
        "reviewResult": "Approve",
        "status": "Completed",
        "assignedToMe": true,
        "justification": "Admin consent granted.",
        "reviewedBy": {
          "id": "00000001-0000-0000-c000-000000000000",
          "displayName": "",
          "userPrincipalName": "",
          "mail": ""
        }
      }
    ]
  },
  "approvalId": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
  "completedDateTime": null,
  "customData": null
}
```
