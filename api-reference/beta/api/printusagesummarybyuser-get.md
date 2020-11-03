---
title: Obter printUsageSummaryByUser
description: Recupere o resumo de uso de um usuário para um determinado período de tempo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7c7ec996054461b2b2eeb201656c018a5796d5bc
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848784"
---
# <a name="get-printusagesummarybyuser"></a><span data-ttu-id="3feee-103">Obter printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="3feee-103">Get printUsageSummaryByUser</span></span>

<span data-ttu-id="3feee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3feee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3feee-105">Recupere o resumo de uso de um usuário para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="3feee-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="3feee-106">Consulte a documentação do [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) para obter descrições de cada ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="3feee-106">See the [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="3feee-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3feee-107">Permissions</span></span>
<span data-ttu-id="3feee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3feee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3feee-110">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="3feee-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="3feee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3feee-111">Permission type</span></span> | <span data-ttu-id="3feee-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3feee-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3feee-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3feee-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3feee-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3feee-114">Reports.Read.All</span></span> |
|<span data-ttu-id="3feee-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3feee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3feee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3feee-116">Not Supported.</span></span>|
|<span data-ttu-id="3feee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3feee-117">Application</span></span>|<span data-ttu-id="3feee-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3feee-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3feee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3feee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser/{id}
GET /reports/monthlyPrintUsageSummariesByUser/{id}
GET /print/reports/dailyPrintUsageSummariesByUser/{id}
GET /print/reports/monthlyPrintUsageSummariesByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3feee-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3feee-120">Optional query parameters</span></span>
<span data-ttu-id="3feee-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3feee-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3feee-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3feee-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3feee-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3feee-123">Request headers</span></span>
| <span data-ttu-id="3feee-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3feee-124">Name</span></span>      |<span data-ttu-id="3feee-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3feee-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3feee-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3feee-126">Authorization</span></span> | <span data-ttu-id="3feee-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3feee-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3feee-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3feee-129">Request body</span></span>
<span data-ttu-id="3feee-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3feee-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3feee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3feee-131">Response</span></span>
<span data-ttu-id="3feee-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3feee-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3feee-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3feee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3feee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3feee-134">Request</span></span>
<span data-ttu-id="3feee-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3feee-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByUser"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser/{id}
```
##### <a name="response"></a><span data-ttu-id="3feee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3feee-136">Response</span></span>
<span data-ttu-id="3feee-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3feee-137">The following is an example of the response.</span></span>
><span data-ttu-id="3feee-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3feee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@microsoft.com",
  "usageDate": "2020-02-04T00:00:00.0000000Z",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageSummaryByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

