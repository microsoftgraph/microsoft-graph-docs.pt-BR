---
title: Listar dadosSource
description: Obter os recursos dataSource da propriedade de navegação dataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 60cec935db8e451efa6e855c56b71eb026ca4f99
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080706"
---
# <a name="list-datasource"></a><span data-ttu-id="238cc-103">Listar dadosSource</span><span class="sxs-lookup"><span data-stu-id="238cc-103">List dataSource</span></span>

<span data-ttu-id="238cc-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="238cc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="238cc-105">Obter a lista de dadosSources associados a uma fonte de dados não custodial.</span><span class="sxs-lookup"><span data-stu-id="238cc-105">Get the list of dataSources associated with a non-custodial data source.</span></span>

## <a name="permissions"></a><span data-ttu-id="238cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="238cc-106">Permissions</span></span>

<span data-ttu-id="238cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="238cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="238cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="238cc-109">Permission type</span></span>|<span data-ttu-id="238cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="238cc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="238cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="238cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="238cc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238cc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="238cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="238cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="238cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="238cc-114">Not supported.</span></span>|
|<span data-ttu-id="238cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="238cc-115">Application</span></span>|<span data-ttu-id="238cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="238cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="238cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="238cc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/dataSource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="238cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="238cc-118">Optional query parameters</span></span>

<span data-ttu-id="238cc-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="238cc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="238cc-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="238cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="238cc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="238cc-121">Request headers</span></span>

|<span data-ttu-id="238cc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="238cc-122">Name</span></span>|<span data-ttu-id="238cc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="238cc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="238cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="238cc-124">Authorization</span></span>|<span data-ttu-id="238cc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="238cc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="238cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="238cc-127">Request body</span></span>

<span data-ttu-id="238cc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="238cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="238cc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="238cc-129">Response</span></span>

<span data-ttu-id="238cc-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="238cc-130">If successful, this method returns a `200 OK` response code and a collection of [dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="238cc-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="238cc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="238cc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="238cc-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/datasource
```

### <a name="response"></a><span data-ttu-id="238cc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="238cc-133">Response</span></span>

<span data-ttu-id="238cc-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="238cc-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources('8e402dd7f3c94a3abc086e5d07db1c6d')/dataSource/$entity",
        "@odata.type": "#microsoft.graph.ediscovery.userSource",
        "displayName": "Adele Vance",
        "createdDateTime": "2021-02-17T19:41:22.5902664Z",
        "id": "8e402dd7f3c94a3abc086e5d07db1c6d",
        "email": "AdeleV@contoso.com",
        "includedSources": "mailbox",
        "createdBy": {
            "user": {
                "id": "ediscovery admin",
                "displayName": "c1db6f13-332a-4d84-b111-914383ff9fc9"
            }
        }
      }
  ]

}
```
