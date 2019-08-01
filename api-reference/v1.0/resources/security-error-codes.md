---
title: Respostas de erro da API de segurança do Microsoft Graph
description: Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 2d77a0f21623a98e4041b845e92a23c7574a415d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034465"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="37a6b-103">Respostas de erro da API de segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="37a6b-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="37a6b-104">Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="37a6b-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="37a6b-105">Erros</span><span class="sxs-lookup"><span data-stu-id="37a6b-105">Errors</span></span>

<span data-ttu-id="37a6b-106">A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados.</span><span class="sxs-lookup"><span data-stu-id="37a6b-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="37a6b-107">Quando um erro HTTP é recebido pela API de segurança do Microsoft Graph, ele envia de volta um cabeçalho de aviso no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="37a6b-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="37a6b-108">Esse cabeçalho de aviso é enviado de volta aos clientes quando um dos provedores de dados retorna um código de erro diferente de 2xx ou 404.</span><span class="sxs-lookup"><span data-stu-id="37a6b-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="37a6b-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="37a6b-109">For example:</span></span>

- <span data-ttu-id="37a6b-110">HttpStatusCode. proibido (403) poderá ser retornado se o acesso ao recurso não for concedido.</span><span class="sxs-lookup"><span data-stu-id="37a6b-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="37a6b-111">Se um provedor expirar, HttpStatusCode. GatewayTimeout (504) será retornado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="37a6b-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="37a6b-112">Se ocorrer um erro de provedor interno, HttpStatusCode. InternalServerError (500) será usado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="37a6b-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="37a6b-113">Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no cabeçalho de aviso porque esses códigos são esperados para êxito ou quando os dados não são encontrados, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="37a6b-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="37a6b-114">Em um sistema federado, um 404 não encontrado é esperado quantas vezes os dados são conhecidos apenas por um ou vários provedores.</span><span class="sxs-lookup"><span data-stu-id="37a6b-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="37a6b-115">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37a6b-115">Example</span></span>

<span data-ttu-id="37a6b-116">Um usuário solicita `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="37a6b-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="37a6b-117">Como 404 e 200 são condições esperadas, o cabeçalho de aviso contém o seguinte:</span><span class="sxs-lookup"><span data-stu-id="37a6b-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="37a6b-118">**Observação:** Cada cabeçalho HTTP é uma coleção de subitens, de forma que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="37a6b-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="37a6b-119">Restrições</span><span class="sxs-lookup"><span data-stu-id="37a6b-119">Constraints</span></span>

<span data-ttu-id="37a6b-120">O `$top` parâmetro de consulta OData tem um limite de 1000 alertas e uma combinação de `$top`  +  `$skip` parâmetros de consulta OData não pode exceder 6000 alertas.</span><span class="sxs-lookup"><span data-stu-id="37a6b-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="37a6b-121">Por exemplo, `/security/alerts?$top=10&$skip=5990` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=5991` retornará um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="37a6b-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="37a6b-122">Uma solução alternativa para esse limite é usar o `$filter` parâmetro de consulta OData com o `eventDateTime` da entidade de alerta da API de segurança do Microsoft Graph, usando `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` e substituindo o valor DateTime pelo último alerta (6000th).</span><span class="sxs-lookup"><span data-stu-id="37a6b-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="37a6b-123">Você também pode definir um intervalo para o `eventDateTime`; por exemplo, *alertas? $Filter = eventDateTime **gt** 2018-11-**11**T00:00:00.000 z&eventDateTime **lt** 2018-11-**12**T00:00:00.000 z*</span><span class="sxs-lookup"><span data-stu-id="37a6b-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="37a6b-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="37a6b-124">See also</span></span>

<span data-ttu-id="37a6b-125">Se você estiver tendo problemas com a autorização, confira [autorização e a API de segurança do Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="37a6b-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
