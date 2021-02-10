---
title: Listar userSources
description: Obter uma lista dos objetos userSource e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 2812fe2bfbcd6540462122dcfcaddaee8c54ca9b
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176570"
---
# <a name="list-usersources"></a><span data-ttu-id="5000d-103">Listar userSources</span><span class="sxs-lookup"><span data-stu-id="5000d-103">List userSources</span></span>

<span data-ttu-id="5000d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5000d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5000d-105">Obter uma lista dos [objetos userSource](../resources/usersource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="5000d-105">Get a list of the [userSource](../resources/usersource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5000d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5000d-106">Permissions</span></span>

<span data-ttu-id="5000d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5000d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5000d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5000d-109">Permission type</span></span>|<span data-ttu-id="5000d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5000d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5000d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5000d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5000d-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="5000d-112">User.Read</span></span>|
|<span data-ttu-id="5000d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5000d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5000d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5000d-114">Not supported.</span></span>|
|<span data-ttu-id="5000d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5000d-115">Application</span></span>|<span data-ttu-id="5000d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5000d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5000d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5000d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5000d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5000d-118">Optional query parameters</span></span>

<span data-ttu-id="5000d-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5000d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5000d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5000d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5000d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5000d-121">Request headers</span></span>

|<span data-ttu-id="5000d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5000d-122">Name</span></span>|<span data-ttu-id="5000d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5000d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5000d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5000d-124">Authorization</span></span>|<span data-ttu-id="5000d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5000d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5000d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5000d-127">Request body</span></span>

<span data-ttu-id="5000d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5000d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5000d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5000d-129">Response</span></span>

<span data-ttu-id="5000d-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos userSource](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5000d-130">If successful, this method returns a `200 OK` response code and a collection of [userSource](../resources/usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5000d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5000d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5000d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5000d-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5000d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5000d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
```
# <a name="c"></a>[<span data-ttu-id="5000d-134">C#</span><span class="sxs-lookup"><span data-stu-id="5000d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5000d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5000d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5000d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5000d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5000d-137">Java</span><span class="sxs-lookup"><span data-stu-id="5000d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5000d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5000d-138">Response</span></span>

<span data-ttu-id="5000d-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5000d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
