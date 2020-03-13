---
title: Respostas de erro da API de segurança do Microsoft Graph
description: Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 1faba5ca71fe9478963120ec43d9eb9da08d721a
ms.sourcegitcommit: 8a84ee922acd2946a3ffae9f8f7f7b485567bc05
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2020
ms.locfileid: "42618907"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="f2e9f-103">Respostas de erro da API de segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f2e9f-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="f2e9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2e9f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2e9f-105">Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-105">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="f2e9f-106">Erros</span><span class="sxs-lookup"><span data-stu-id="f2e9f-106">Errors</span></span>

<span data-ttu-id="f2e9f-107">A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-107">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="f2e9f-108">Quando um erro HTTP é recebido pela API de segurança do Microsoft Graph, ele envia de volta um cabeçalho de aviso no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="f2e9f-108">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="f2e9f-109">Esse cabeçalho de aviso é enviado de volta aos clientes quando um dos provedores de dados retorna um código de erro diferente de 2xx ou 404.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-109">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="f2e9f-110">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="f2e9f-110">For example:</span></span>

- <span data-ttu-id="f2e9f-111">HttpStatusCode. proibido (403) poderá ser retornado se o acesso ao recurso não for concedido.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-111">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="f2e9f-112">Se um provedor expirar, HttpStatusCode. GatewayTimeout (504) será retornado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-112">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="f2e9f-113">Se ocorrer um erro de provedor interno, HttpStatusCode. InternalServerError (500) será usado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-113">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="f2e9f-114">Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no cabeçalho de aviso porque esses códigos são esperados para êxito ou quando os dados não são encontrados, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-114">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="f2e9f-115">Em um sistema federado, um 404 não encontrado é esperado quantas vezes os dados são conhecidos apenas por um ou vários provedores.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-115">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="f2e9f-116">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2e9f-116">Example</span></span>

<span data-ttu-id="f2e9f-117">Um usuário solicita `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-117">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="f2e9f-118">Como 404 e 200 são condições esperadas, o cabeçalho de aviso contém o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f2e9f-118">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="f2e9f-119">**Observação:** Cada cabeçalho HTTP é uma coleção de subitens, de forma que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-119">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="threat-indicator-bulk-action-errors"></a><span data-ttu-id="f2e9f-120">Erros de ação em massa do indicador de ameaça</span><span class="sxs-lookup"><span data-stu-id="f2e9f-120">Threat indicator bulk action errors</span></span>

<span data-ttu-id="f2e9f-121">As ações em massa (criar, atualizar, excluir) podem gerar dois códigos de erro potenciais diferentes:</span><span class="sxs-lookup"><span data-stu-id="f2e9f-121">Bulk actions (create, update, delete) can generate two different potential error codes:</span></span>

- <span data-ttu-id="f2e9f-122">Um código de erro 400 indica que o corpo fornecido teve um erro durante a serialização.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-122">A 400 error code indicates that the body provided had an error during serialization.</span></span>
- <span data-ttu-id="f2e9f-123">Um código de erro 206 indica que uma ou mais ações em massa falharam quando foram federadas no provedor.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-123">A 206 error code indicates that one or more of the bulk actions failed when it was federated out to its provider.</span></span> <span data-ttu-id="f2e9f-124">A resposta conterá dados de sucesso/erro dos provedores individuais para cada indicador de inteligência de ameaças.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-124">The response will contain success/error data from the individual providers for each threat intelligence indicator.</span></span> <span data-ttu-id="f2e9f-125">Ao contrário dos [alertas](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), todas as informações de erro em potencial serão contidas no corpo da resposta para ações em massa [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) .</span><span class="sxs-lookup"><span data-stu-id="f2e9f-125">Unlike [alerts](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), all potential error information will be contained within the body of the response for [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) bulk actions.</span></span>

## <a name="constraints"></a><span data-ttu-id="f2e9f-126">Restrições</span><span class="sxs-lookup"><span data-stu-id="f2e9f-126">Constraints</span></span>

<span data-ttu-id="f2e9f-127">O `$top` parâmetro de consulta OData tem um limite de 1000 alertas.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-127">The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="f2e9f-128">É recomendável incluir apenas o `$top` e não o `$skip` na primeira consulta OBTER.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-128">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="f2e9f-129">Você pode usar `@odata.nextLink` para paginação.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-129">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="f2e9f-130">Se você precisar usar o `$skip`, ele tem um limite de 500 alertas.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-130">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="f2e9f-131">Por exemplo, `/security/alerts?$top=10&$skip=500` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=501` retornará um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-131">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="f2e9f-132">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="f2e9f-132">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

<span data-ttu-id="f2e9f-133">Uma solução alternativa para esse limite é usar o `$filter` parâmetro de consulta OData com `eventDateTime` a entidade de alerta da API de segurança do Microsoft Graph, `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` usando e substituindo o valor DateTime pelo último alerta (1500th).</span><span class="sxs-lookup"><span data-stu-id="f2e9f-133">A workaround for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (1500th) alert.</span></span> <span data-ttu-id="f2e9f-134">Você também pode definir um intervalo para o `eventDateTime`; por exemplo, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z`.</span><span class="sxs-lookup"><span data-stu-id="f2e9f-134">You can also set a range for the `eventDateTime`; for example, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z`.</span></span>

## <a name="see-also"></a><span data-ttu-id="f2e9f-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="f2e9f-135">See also</span></span>

<span data-ttu-id="f2e9f-136">Se você estiver tendo problemas com a autorização, confira [autorização e a API de segurança do Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="f2e9f-136">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
