---
title: Obter connectionOperation
description: Leia as propriedades e as relações de um objeto connectionOperation.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7a5e5849e91b0d7816ba6b293838eb434e05c900
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467232"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="12ea6-103">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="12ea6-103">Get connectionOperation</span></span>

<span data-ttu-id="12ea6-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="12ea6-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="12ea6-105">Leia as propriedades e as relações de um [objeto connectionOperation.](../resources/externalconnectors-connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="12ea6-105">Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12ea6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12ea6-106">Permissions</span></span>
<span data-ttu-id="12ea6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12ea6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12ea6-109">Permission type</span></span>|<span data-ttu-id="12ea6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12ea6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12ea6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12ea6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12ea6-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="12ea6-112">Not applicable</span></span>|
|<span data-ttu-id="12ea6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12ea6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12ea6-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="12ea6-114">Not applicable</span></span>|
|<span data-ttu-id="12ea6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12ea6-115">Application</span></span>| <span data-ttu-id="12ea6-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="12ea6-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="12ea6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12ea6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/operations/{connectionOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12ea6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12ea6-118">Optional query parameters</span></span>
<span data-ttu-id="12ea6-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12ea6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="12ea6-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="12ea6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="12ea6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea6-121">Request headers</span></span>
|<span data-ttu-id="12ea6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="12ea6-122">Name</span></span>|<span data-ttu-id="12ea6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ea6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12ea6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="12ea6-124">Authorization</span></span>|<span data-ttu-id="12ea6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12ea6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12ea6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea6-127">Request body</span></span>
<span data-ttu-id="12ea6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12ea6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12ea6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ea6-129">Response</span></span>

<span data-ttu-id="12ea6-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [connectionOperation](../resources/externalconnectors-connectionoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12ea6-130">If successful, this method returns a `200 OK` response code and a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12ea6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="12ea6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12ea6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea6-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```


### <a name="response"></a><span data-ttu-id="12ea6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ea6-133">Response</span></span>
<span data-ttu-id="12ea6-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="12ea6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

