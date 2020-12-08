---
title: Obter usuário
description: Leia as propriedades e os relacionamentos de um objeto username.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 653c5d45286cfd860dff1397b5ecb65fe23bd992
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597506"
---
# <a name="get-usersource"></a><span data-ttu-id="1b4e8-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="1b4e8-103">Get userSource</span></span>

<span data-ttu-id="1b4e8-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1b4e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b4e8-105">Leia as propriedades e os relacionamentos de um objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="1b4e8-105">Read the properties and relationships of a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b4e8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1b4e8-106">Permissions</span></span>

<span data-ttu-id="1b4e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b4e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b4e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b4e8-109">Permission type</span></span>|<span data-ttu-id="1b4e8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b4e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b4e8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b4e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b4e8-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="1b4e8-112">User.Read</span></span>|
|<span data-ttu-id="1b4e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b4e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b4e8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-114">Not supported.</span></span>|
|<span data-ttu-id="1b4e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b4e8-115">Application</span></span>|<span data-ttu-id="1b4e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b4e8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b4e8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b4e8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b4e8-118">Optional query parameters</span></span>

<span data-ttu-id="1b4e8-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1b4e8-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b4e8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b4e8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b4e8-121">Request headers</span></span>

|<span data-ttu-id="1b4e8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1b4e8-122">Name</span></span>|<span data-ttu-id="1b4e8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b4e8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b4e8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b4e8-124">Authorization</span></span>|<span data-ttu-id="1b4e8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b4e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b4e8-127">Request body</span></span>

<span data-ttu-id="1b4e8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b4e8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b4e8-129">Response</span></span>

<span data-ttu-id="1b4e8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [username](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-130">If successful, this method returns a `200 OK` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b4e8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b4e8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b4e8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b4e8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```

### <a name="response"></a><span data-ttu-id="1b4e8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b4e8-133">Response</span></span>

<span data-ttu-id="1b4e8-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b4e8-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/userSources",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-08-21T13:20:01.3430206Z",
    "id": "46384443-4137-3032-3437-363939433735",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "Adele Vance"
        }
    }
}
```
