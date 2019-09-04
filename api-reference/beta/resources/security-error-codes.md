---
title: Respostas de erro da API de segurança do Microsoft Graph
description: Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 2291f0009c7d54a62ac30d448a9f97ff8935a569
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726309"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="261cc-103">Respostas de erro da API de segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="261cc-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="261cc-104">Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="261cc-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="261cc-105">Erros</span><span class="sxs-lookup"><span data-stu-id="261cc-105">Errors</span></span>

<span data-ttu-id="261cc-106">A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados.</span><span class="sxs-lookup"><span data-stu-id="261cc-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="261cc-107">Quando um erro HTTP é recebido pela API de segurança do Microsoft Graph, ele envia de volta um cabeçalho de aviso no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="261cc-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="261cc-108">Esse cabeçalho de aviso é enviado de volta aos clientes quando um dos provedores de dados retorna um código de erro diferente de 2xx ou 404.</span><span class="sxs-lookup"><span data-stu-id="261cc-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="261cc-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="261cc-109">For example:</span></span>

- <span data-ttu-id="261cc-110">HttpStatusCode. proibido (403) poderá ser retornado se o acesso ao recurso não for concedido.</span><span class="sxs-lookup"><span data-stu-id="261cc-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="261cc-111">Se um provedor expirar, HttpStatusCode. GatewayTimeout (504) será retornado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="261cc-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="261cc-112">Se ocorrer um erro de provedor interno, HttpStatusCode. InternalServerError (500) será usado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="261cc-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="261cc-113">Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no cabeçalho de aviso porque esses códigos são esperados para êxito ou quando os dados não são encontrados, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="261cc-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="261cc-114">Em um sistema federado, um 404 não encontrado é esperado quantas vezes os dados são conhecidos apenas por um ou vários provedores.</span><span class="sxs-lookup"><span data-stu-id="261cc-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="261cc-115">Exemplo</span><span class="sxs-lookup"><span data-stu-id="261cc-115">Example</span></span>

<span data-ttu-id="261cc-116">Um usuário solicita `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="261cc-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="261cc-117">Como 404 e 200 são condições esperadas, o cabeçalho de aviso contém o seguinte:</span><span class="sxs-lookup"><span data-stu-id="261cc-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="261cc-118">**Observação:** Cada cabeçalho HTTP é uma coleção de subitens, de forma que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="261cc-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="threat-indicator-bulk-action-errors"></a><span data-ttu-id="261cc-119">Erros de ação em massa do indicador de ameaça</span><span class="sxs-lookup"><span data-stu-id="261cc-119">Threat Indicator Bulk Action Errors</span></span>

<span data-ttu-id="261cc-120">Ações em massa (ou seja, criar, atualizar e excluir) podem gerar dois códigos de erro potenciais diferentes.</span><span class="sxs-lookup"><span data-stu-id="261cc-120">Bulk actions (i.e. creating, updating, and deleting) can generate two different potential error codes.</span></span>  <span data-ttu-id="261cc-121">Um código de erro 400 indica que o corpo fornecido teve um erro durante a serialização, enquanto um código de erro 206 indica que uma ou mais das ações em massa falharam ao serem federadas no provedor.</span><span class="sxs-lookup"><span data-stu-id="261cc-121">A 400 error code indicates that the body provided had an error during serialization, while a 206 error code indicates that one or more of the bulk actions failed when it was federated out to its provider.</span></span> <span data-ttu-id="261cc-122">A resposta conterá dados de sucesso/erro dos provedores individuais para cada indicador de inteligência de ameaças.</span><span class="sxs-lookup"><span data-stu-id="261cc-122">The response will contain success/error data from the individual providers for each Threat Intelligence indicator.</span></span> <span data-ttu-id="261cc-123">Diferentemente de alertas, todas as informações de erro em potencial serão contidas no corpo da resposta para ações em massa de indicador de ameaça.</span><span class="sxs-lookup"><span data-stu-id="261cc-123">Unlike with Alerts, all potential error information will be contained within the body of the response for Threat Indicator bulk actions.</span></span>

## <a name="constraints"></a><span data-ttu-id="261cc-124">Restrições</span><span class="sxs-lookup"><span data-stu-id="261cc-124">Constraints</span></span>

<span data-ttu-id="261cc-125">O `$top` parâmetro de consulta OData tem um limite de 1000 alertas e uma combinação de `$top`  +  `$skip` parâmetros de consulta OData não pode exceder 6000 alertas.</span><span class="sxs-lookup"><span data-stu-id="261cc-125">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="261cc-126">Por exemplo, `/security/alerts?$top=10&$skip=5990` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=5991` retornará um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="261cc-126">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="261cc-127">Uma solução alternativa para esse limite é usar o `$filter` parâmetro de consulta OData com o `eventDateTime` da entidade de alerta da API de segurança do Microsoft Graph, usando `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` e substituindo o valor DateTime pelo último alerta (6000th).</span><span class="sxs-lookup"><span data-stu-id="261cc-127">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="261cc-128">Você também pode definir um intervalo para o `eventDateTime`; por exemplo, *alertas? $Filter = eventDateTime **gt** 2018-11-**11**T00:00:00.000 z&eventDateTime **lt** 2018-11-**12**T00:00:00.000 z*</span><span class="sxs-lookup"><span data-stu-id="261cc-128">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="261cc-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="261cc-129">See also</span></span>

<span data-ttu-id="261cc-130">Se você estiver tendo problemas com a autorização, confira [autorização e a API de segurança do Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="261cc-130">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
