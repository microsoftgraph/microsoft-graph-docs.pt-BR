---
title: Obter riskyUser
description: Leia as propriedades e as relações de um objeto riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc7b7758b7d368ffe248cbfe57c29c98955b3ef6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440028"
---
# <a name="get-riskyuser"></a><span data-ttu-id="5b4f4-103">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="5b4f4-103">Get riskyUser</span></span>
<span data-ttu-id="5b4f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b4f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b4f4-105">Leia as propriedades e as relações de um [objeto riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5b4f4-105">Read the properties and relationships of a [riskyUser](../resources/riskyuser.md) object.</span></span>

><span data-ttu-id="5b4f4-106">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b4f4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b4f4-107">Permissions</span></span>
<span data-ttu-id="5b4f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5b4f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="5b4f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b4f4-110">Permission type</span></span>      | <span data-ttu-id="5b4f4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b4f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b4f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b4f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b4f4-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4f4-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="5b4f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b4f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b4f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-115">Not supported.</span></span>    |
|<span data-ttu-id="5b4f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b4f4-116">Application</span></span> | <span data-ttu-id="5b4f4-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4f4-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b4f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b4f4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b4f4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b4f4-119">Optional query parameters</span></span>
<span data-ttu-id="5b4f4-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5b4f4-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5b4f4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b4f4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4f4-122">Request headers</span></span>
|<span data-ttu-id="5b4f4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5b4f4-123">Name</span></span>|<span data-ttu-id="5b4f4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b4f4-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b4f4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b4f4-125">Authorization</span></span>|<span data-ttu-id="5b4f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b4f4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4f4-128">Request body</span></span>
<span data-ttu-id="5b4f4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b4f4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b4f4-130">Response</span></span>

<span data-ttu-id="5b4f4-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b4f4-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b4f4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b4f4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4f4-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```


### <a name="response"></a><span data-ttu-id="5b4f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b4f4-134">Response</span></span>
<span data-ttu-id="5b4f4-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5b4f4-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUser",
      "id": "d1d4a5d4-a5d4-d1d4-d4a5-d4d1d4a5d4d1",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String"
    }
  ]
}
```


