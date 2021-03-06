---
title: Obter userSource
description: Leia as propriedades e as relações de um objeto userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01ad2f83682ac786f35f423fa387293face51114
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515986"
---
# <a name="get-usersource"></a><span data-ttu-id="ef086-103">Obter userSource</span><span class="sxs-lookup"><span data-stu-id="ef086-103">Get userSource</span></span>

<span data-ttu-id="ef086-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ef086-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef086-105">Leia as propriedades e as relações de um [objeto userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="ef086-105">Read the properties and relationships of a [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef086-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef086-106">Permissions</span></span>

<span data-ttu-id="ef086-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef086-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef086-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef086-109">Permission type</span></span>|<span data-ttu-id="ef086-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef086-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef086-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef086-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef086-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef086-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ef086-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef086-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef086-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef086-114">Not supported.</span></span>|
|<span data-ttu-id="ef086-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef086-115">Application</span></span>|<span data-ttu-id="ef086-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef086-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef086-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef086-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef086-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ef086-118">Optional query parameters</span></span>

<span data-ttu-id="ef086-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef086-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ef086-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ef086-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef086-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef086-121">Request headers</span></span>

|<span data-ttu-id="ef086-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ef086-122">Name</span></span>|<span data-ttu-id="ef086-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef086-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef086-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef086-124">Authorization</span></span>|<span data-ttu-id="ef086-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef086-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef086-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef086-127">Request body</span></span>

<span data-ttu-id="ef086-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef086-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef086-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef086-129">Response</span></span>

<span data-ttu-id="ef086-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef086-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef086-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ef086-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef086-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef086-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ef086-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef086-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="ef086-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef086-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef086-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef086-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef086-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef086-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef086-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef086-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ef086-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef086-138">Response</span></span>

<span data-ttu-id="ef086-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef086-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
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
