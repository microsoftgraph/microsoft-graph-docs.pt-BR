---
title: Obter appConsentRequest
description: Leia as propriedades e as relações de um objeto appConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8c8d27d86312ac87b891fbe5c66c0b90de2f9219
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750977"
---
# <a name="get-appconsentrequest"></a><span data-ttu-id="07c4d-103">Obter appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="07c4d-103">Get appConsentRequest</span></span>
<span data-ttu-id="07c4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c4d-105">Leia as propriedades e as relações de um [objeto appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="07c4d-105">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c4d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="07c4d-106">Permissions</span></span>
<span data-ttu-id="07c4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c4d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07c4d-109">Permission type</span></span>|<span data-ttu-id="07c4d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07c4d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c4d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07c4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="07c4d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c4d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="07c4d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07c4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c4d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c4d-114">Not supported.</span></span>|
|<span data-ttu-id="07c4d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07c4d-115">Application</span></span>|<span data-ttu-id="07c4d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c4d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c4d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07c4d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07c4d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07c4d-118">Optional query parameters</span></span>
<span data-ttu-id="07c4d-119">Este método dá suporte ao  `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07c4d-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="07c4d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="07c4d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="07c4d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07c4d-121">Request headers</span></span>
|<span data-ttu-id="07c4d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="07c4d-122">Name</span></span>|<span data-ttu-id="07c4d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="07c4d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="07c4d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="07c4d-124">Authorization</span></span>|<span data-ttu-id="07c4d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07c4d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07c4d-127">Request body</span></span>
<span data-ttu-id="07c4d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07c4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07c4d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c4d-129">Response</span></span>

<span data-ttu-id="07c4d-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07c4d-130">If successful, this method returns a `200 OK` response code and an [appConsentRequest](../resources/appconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07c4d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="07c4d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07c4d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07c4d-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="07c4d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="07c4d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed
```
# <a name="c"></a>[<span data-ttu-id="07c4d-134">C#</span><span class="sxs-lookup"><span data-stu-id="07c4d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appconsentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07c4d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07c4d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appconsentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07c4d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07c4d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appconsentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07c4d-137">Java</span><span class="sxs-lookup"><span data-stu-id="07c4d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appconsentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="07c4d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c4d-138">Response</span></span>
><span data-ttu-id="07c4d-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="07c4d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

