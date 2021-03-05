---
title: Listar riskyUsers
description: Obter uma lista dos objetos riskyUser e suas propriedades.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc72c174b81a5d2442b264026305e28cbb03afdf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448057"
---
# <a name="list-riskyusers"></a><span data-ttu-id="ac257-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ac257-103">List riskyUsers</span></span>
<span data-ttu-id="ac257-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac257-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac257-105">Obter uma lista dos [objetos riskyUser](../resources/riskyuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ac257-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac257-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac257-106">Permissions</span></span>
<span data-ttu-id="ac257-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="ac257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="ac257-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac257-109">Permission type</span></span>|<span data-ttu-id="ac257-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac257-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac257-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac257-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ac257-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac257-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="ac257-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac257-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac257-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac257-114">Not supported.</span></span>    |
|<span data-ttu-id="ac257-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac257-115">Application</span></span> | <span data-ttu-id="ac257-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac257-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac257-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac257-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac257-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac257-118">Optional query parameters</span></span>
<span data-ttu-id="ac257-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac257-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ac257-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ac257-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac257-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac257-121">Request headers</span></span>
|<span data-ttu-id="ac257-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ac257-122">Name</span></span>|<span data-ttu-id="ac257-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac257-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac257-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac257-124">Authorization</span></span>|<span data-ttu-id="ac257-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac257-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac257-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac257-127">Request body</span></span>
<span data-ttu-id="ac257-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac257-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac257-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac257-129">Response</span></span>

<span data-ttu-id="ac257-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac257-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac257-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ac257-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac257-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac257-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="ac257-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac257-133">Response</span></span>
<span data-ttu-id="ac257-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ac257-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUser)"
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


