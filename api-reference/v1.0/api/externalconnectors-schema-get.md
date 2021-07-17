---
title: Obter esquema
description: Leia as propriedades e as relações de um objeto de esquema.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f76eb8f174958d8698528e49fffda105c54cc7f4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467208"
---
# <a name="get-schema"></a><span data-ttu-id="8474b-103">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="8474b-103">Get schema</span></span>
<span data-ttu-id="8474b-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="8474b-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="8474b-105">Leia as propriedades e as relações de um [objeto de esquema.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="8474b-105">Read the properties and relationships of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8474b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8474b-106">Permissions</span></span>
<span data-ttu-id="8474b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8474b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8474b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8474b-109">Permission type</span></span>|<span data-ttu-id="8474b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8474b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8474b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8474b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8474b-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="8474b-112">Not applicable</span></span>|
|<span data-ttu-id="8474b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8474b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8474b-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="8474b-114">Not applicable</span></span>|
|<span data-ttu-id="8474b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8474b-115">Application</span></span>| <span data-ttu-id="8474b-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="8474b-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="8474b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8474b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8474b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8474b-118">Optional query parameters</span></span>
<span data-ttu-id="8474b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8474b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8474b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8474b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8474b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8474b-121">Request headers</span></span>
|<span data-ttu-id="8474b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8474b-122">Name</span></span>|<span data-ttu-id="8474b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8474b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8474b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8474b-124">Authorization</span></span>|<span data-ttu-id="8474b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8474b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8474b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8474b-127">Request body</span></span>
<span data-ttu-id="8474b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8474b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8474b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8474b-129">Response</span></span>

<span data-ttu-id="8474b-130">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [de esquema](../resources/externalconnectors-schema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8474b-130">If successful, this method returns a `200 OK` response code and a [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8474b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8474b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8474b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8474b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schema"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr/schema
```


### <a name="response"></a><span data-ttu-id="8474b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8474b-133">Response</span></span>
<span data-ttu-id="8474b-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8474b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "baseType": "String",
    "properties": [
      {
        "name": "ticketTitle",
        "type": "string",
        "isSearchable": true,
        "isRetrievable": true,
        "labels": [
          "title"
        ]
      },
      {
        "name": "priority",
        "type": "string",
        "isQueryable": true,
        "isRetrievable": true,
        "isRefinable": true,
        "isSearchable": false
      },
      {
        "name": "assignee",
        "type": "string",
        "isRetrievable": true
      }
    ]
  }
}
```

