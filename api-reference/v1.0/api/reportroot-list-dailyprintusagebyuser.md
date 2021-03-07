---
title: Listar dailyPrintUsageByUser
description: Recupere uma lista de resumos diários de uso de impressão, agrupados pelo usuário.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a1d969acb92a0ffcce069f50c146887724d81f1e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517049"
---
# <a name="list-dailyprintusagebyuser"></a><span data-ttu-id="162bf-103">Listar dailyPrintUsageByUser</span><span class="sxs-lookup"><span data-stu-id="162bf-103">List dailyPrintUsageByUser</span></span>
<span data-ttu-id="162bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="162bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="162bf-105">Recupere uma lista de resumos diários de uso de impressão, agrupados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="162bf-105">Retrieve a list of daily print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="162bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="162bf-106">Permissions</span></span>
<span data-ttu-id="162bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="162bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="162bf-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="162bf-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="162bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="162bf-110">Permission type</span></span> | <span data-ttu-id="162bf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="162bf-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="162bf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="162bf-112">Delegated (work or school account)</span></span>| <span data-ttu-id="162bf-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="162bf-113">Reports.Read.All</span></span> |
|<span data-ttu-id="162bf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="162bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="162bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="162bf-115">Not Supported.</span></span>|
|<span data-ttu-id="162bf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="162bf-116">Application</span></span>|<span data-ttu-id="162bf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="162bf-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="162bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="162bf-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="162bf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="162bf-119">Optional query parameters</span></span>
<span data-ttu-id="162bf-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="162bf-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="162bf-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="162bf-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="162bf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="162bf-122">Request headers</span></span>
|<span data-ttu-id="162bf-123">Nome</span><span class="sxs-lookup"><span data-stu-id="162bf-123">Name</span></span>|<span data-ttu-id="162bf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="162bf-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="162bf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="162bf-125">Authorization</span></span>|<span data-ttu-id="162bf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="162bf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="162bf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="162bf-128">Request body</span></span>
<span data-ttu-id="162bf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="162bf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="162bf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="162bf-130">Response</span></span>

<span data-ttu-id="162bf-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageByUser](../resources/printusagebyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="162bf-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByUser](../resources/printusagebyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="162bf-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="162bf-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="162bf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="162bf-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printusagebyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByUser
```


### <a name="response"></a><span data-ttu-id="162bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="162bf-134">Response</span></span>
<span data-ttu-id="162bf-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="162bf-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printUsageByUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "userPrincipalName": "username@contoso.com",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

