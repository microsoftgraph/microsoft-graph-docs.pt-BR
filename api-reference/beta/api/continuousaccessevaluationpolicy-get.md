---
title: Obter continuousAccessEvaluationPolicy
description: Ler as propriedades de um objeto continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bea54ea801ee9d41314f1fbd2c87070ac4e92773
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023403"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="4960f-103">Obter continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="4960f-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="4960f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4960f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4960f-105">Leia as propriedades e os relacionamentos de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4960f-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4960f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4960f-106">Permissions</span></span>
<span data-ttu-id="4960f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4960f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4960f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4960f-109">Permission type</span></span>|<span data-ttu-id="4960f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4960f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4960f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4960f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4960f-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="4960f-112">Policy.Read.All</span></span> |
|<span data-ttu-id="4960f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4960f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4960f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4960f-114">Not supported.</span></span> |
|<span data-ttu-id="4960f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4960f-115">Application</span></span>                            | <span data-ttu-id="4960f-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="4960f-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4960f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4960f-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4960f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4960f-118">Optional query parameters</span></span>
<span data-ttu-id="4960f-119">Este método dá suporte ao parâmetro de consulta OData ' $select ' para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4960f-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="4960f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4960f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4960f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4960f-121">Request headers</span></span>
|<span data-ttu-id="4960f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4960f-122">Name</span></span>|<span data-ttu-id="4960f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4960f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4960f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4960f-124">Authorization</span></span>|<span data-ttu-id="4960f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4960f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4960f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4960f-127">Request body</span></span>
<span data-ttu-id="4960f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4960f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4960f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4960f-129">Response</span></span>

<span data-ttu-id="4960f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4960f-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4960f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4960f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4960f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4960f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```


### <a name="response"></a><span data-ttu-id="4960f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4960f-133">Response</span></span>

<span data-ttu-id="4960f-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4960f-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
