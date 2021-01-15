---
title: Listar riskyUsers
description: Obter uma lista dos objetos riskyUser e suas propriedades.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 075f135afe075450197ff8b3ed1d8e1c5bbde36d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874344"
---
# <a name="list-riskyusers"></a><span data-ttu-id="310e2-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="310e2-103">List riskyUsers</span></span>
<span data-ttu-id="310e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="310e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="310e2-105">Obter uma lista dos [objetos riskyUser](../resources/riskyuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="310e2-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="310e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="310e2-106">Permissions</span></span>
<span data-ttu-id="310e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="310e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="310e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="310e2-109">Permission type</span></span>|<span data-ttu-id="310e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="310e2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="310e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="310e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="310e2-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="310e2-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="310e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="310e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="310e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="310e2-114">Not supported.</span></span>    |
|<span data-ttu-id="310e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="310e2-115">Application</span></span> | <span data-ttu-id="310e2-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="310e2-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="310e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="310e2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="310e2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="310e2-118">Optional query parameters</span></span>
<span data-ttu-id="310e2-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="310e2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="310e2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="310e2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="310e2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="310e2-121">Request headers</span></span>
|<span data-ttu-id="310e2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="310e2-122">Name</span></span>|<span data-ttu-id="310e2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="310e2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="310e2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="310e2-124">Authorization</span></span>|<span data-ttu-id="310e2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="310e2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="310e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="310e2-127">Request body</span></span>
<span data-ttu-id="310e2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="310e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="310e2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="310e2-129">Response</span></span>

<span data-ttu-id="310e2-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="310e2-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="310e2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="310e2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="310e2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="310e2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="310e2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="310e2-133">Response</span></span>
<span data-ttu-id="310e2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="310e2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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


