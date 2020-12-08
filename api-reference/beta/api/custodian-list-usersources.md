---
title: Listar usersources
description: Obtenha uma lista dos objetos username e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7a73394daea6b870bc1da0ec612ceff1691e3c67
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597493"
---
# <a name="list-usersources"></a><span data-ttu-id="27b99-103">Listar usersources</span><span class="sxs-lookup"><span data-stu-id="27b99-103">List userSources</span></span>

<span data-ttu-id="27b99-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27b99-105">Obtenha uma lista dos objetos [username](../resources/usersource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="27b99-105">Get a list of the [userSource](../resources/usersource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="27b99-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="27b99-106">Permissions</span></span>

<span data-ttu-id="27b99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27b99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27b99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27b99-109">Permission type</span></span>|<span data-ttu-id="27b99-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27b99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27b99-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27b99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27b99-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="27b99-112">User.Read</span></span>|
|<span data-ttu-id="27b99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27b99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27b99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27b99-114">Not supported.</span></span>|
|<span data-ttu-id="27b99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27b99-115">Application</span></span>|<span data-ttu-id="27b99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27b99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27b99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27b99-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27b99-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27b99-118">Optional query parameters</span></span>

<span data-ttu-id="27b99-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27b99-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="27b99-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="27b99-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="27b99-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27b99-121">Request headers</span></span>

|<span data-ttu-id="27b99-122">Nome</span><span class="sxs-lookup"><span data-stu-id="27b99-122">Name</span></span>|<span data-ttu-id="27b99-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="27b99-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27b99-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="27b99-124">Authorization</span></span>|<span data-ttu-id="27b99-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27b99-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27b99-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27b99-127">Request body</span></span>

<span data-ttu-id="27b99-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27b99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27b99-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="27b99-129">Response</span></span>

<span data-ttu-id="27b99-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [username](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27b99-130">If successful, this method returns a `200 OK` response code and a collection of [userSource](../resources/usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27b99-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27b99-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27b99-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27b99-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
```

### <a name="response"></a><span data-ttu-id="27b99-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27b99-133">Response</span></span>

<span data-ttu-id="27b99-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27b99-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/userSources",
    "value": [
        {
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
    ]
}
```
