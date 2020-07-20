---
title: Listar riskyUsers
description: Obtenha uma lista dos objetos riskyUser e suas propriedades.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd6d413803e7461ffe0f00891b6e4db7cd3d0e0b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897551"
---
# <a name="list-riskyusers"></a><span data-ttu-id="cac53-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="cac53-103">List riskyUsers</span></span>
<span data-ttu-id="cac53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cac53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cac53-105">Obtenha uma lista dos objetos [riskyUser](../resources/riskyuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cac53-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cac53-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cac53-106">Permissions</span></span>
<span data-ttu-id="cac53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="cac53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="cac53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cac53-109">Permission type</span></span>|<span data-ttu-id="cac53-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cac53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cac53-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cac53-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cac53-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="cac53-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="cac53-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cac53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cac53-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cac53-114">Not supported.</span></span>    |
|<span data-ttu-id="cac53-115">Application</span><span class="sxs-lookup"><span data-stu-id="cac53-115">Application</span></span> | <span data-ttu-id="cac53-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="cac53-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cac53-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cac53-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cac53-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cac53-118">Optional query parameters</span></span>
<span data-ttu-id="cac53-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cac53-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cac53-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cac53-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cac53-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cac53-121">Request headers</span></span>
|<span data-ttu-id="cac53-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cac53-122">Name</span></span>|<span data-ttu-id="cac53-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cac53-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cac53-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cac53-124">Authorization</span></span>|<span data-ttu-id="cac53-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cac53-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cac53-127">Request body</span></span>
<span data-ttu-id="cac53-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cac53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cac53-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cac53-129">Response</span></span>

<span data-ttu-id="cac53-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cac53-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cac53-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cac53-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cac53-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cac53-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="cac53-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cac53-133">Response</span></span>
<span data-ttu-id="cac53-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cac53-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

