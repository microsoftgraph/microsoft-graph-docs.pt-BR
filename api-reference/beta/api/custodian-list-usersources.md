---
title: Listar userSources
description: Obter uma lista dos objetos userSource e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9f1dba8034b6655a15b00118e161b7ddb454bc2b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872566"
---
# <a name="list-usersources"></a><span data-ttu-id="c5cc0-103">Listar userSources</span><span class="sxs-lookup"><span data-stu-id="c5cc0-103">List userSources</span></span>

<span data-ttu-id="c5cc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5cc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5cc0-105">Obter uma lista dos [objetos userSource](../resources/usersource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-105">Get a list of the [userSource](../resources/usersource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5cc0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5cc0-106">Permissions</span></span>

<span data-ttu-id="c5cc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5cc0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5cc0-109">Permission type</span></span>|<span data-ttu-id="c5cc0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5cc0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5cc0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5cc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c5cc0-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c5cc0-112">User.Read</span></span>|
|<span data-ttu-id="c5cc0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5cc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5cc0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-114">Not supported.</span></span>|
|<span data-ttu-id="c5cc0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5cc0-115">Application</span></span>|<span data-ttu-id="c5cc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5cc0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5cc0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5cc0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5cc0-118">Optional query parameters</span></span>

<span data-ttu-id="c5cc0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c5cc0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c5cc0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5cc0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cc0-121">Request headers</span></span>

|<span data-ttu-id="c5cc0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c5cc0-122">Name</span></span>|<span data-ttu-id="c5cc0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5cc0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5cc0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5cc0-124">Authorization</span></span>|<span data-ttu-id="c5cc0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5cc0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cc0-127">Request body</span></span>

<span data-ttu-id="c5cc0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5cc0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5cc0-129">Response</span></span>

<span data-ttu-id="c5cc0-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos userSource](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-130">If successful, this method returns a `200 OK` response code and a collection of [userSource](../resources/usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5cc0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5cc0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5cc0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cc0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
```

### <a name="response"></a><span data-ttu-id="c5cc0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5cc0-133">Response</span></span>

<span data-ttu-id="c5cc0-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5cc0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
