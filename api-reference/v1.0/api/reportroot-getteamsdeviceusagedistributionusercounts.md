---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 79f0e776426179b63fbe75fd0cfac465927f642f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277186"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="9a97b-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="9a97b-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="9a97b-104">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="9a97b-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a97b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a97b-105">Permissions</span></span>

<span data-ttu-id="9a97b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a97b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a97b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a97b-108">Permission type</span></span>                        | <span data-ttu-id="9a97b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a97b-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9a97b-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a97b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a97b-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a97b-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9a97b-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a97b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a97b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a97b-113">Not supported.</span></span>                           |
| <span data-ttu-id="9a97b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a97b-114">Application</span></span>                            | <span data-ttu-id="9a97b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a97b-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9a97b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a97b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9a97b-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9a97b-117">Function parameters</span></span>

<span data-ttu-id="9a97b-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9a97b-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9a97b-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9a97b-119">Parameter</span></span> | <span data-ttu-id="9a97b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a97b-120">Type</span></span>   | <span data-ttu-id="9a97b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a97b-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9a97b-122">ponto</span><span class="sxs-lookup"><span data-stu-id="9a97b-122">period</span></span>    | <span data-ttu-id="9a97b-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a97b-123">string</span></span> | <span data-ttu-id="9a97b-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9a97b-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9a97b-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9a97b-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9a97b-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9a97b-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9a97b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a97b-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9a97b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a97b-128">Request headers</span></span>

| <span data-ttu-id="9a97b-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9a97b-129">Name</span></span>          | <span data-ttu-id="9a97b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a97b-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9a97b-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a97b-131">Authorization</span></span> | <span data-ttu-id="9a97b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a97b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9a97b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a97b-134">Response</span></span>

<span data-ttu-id="9a97b-135">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9a97b-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9a97b-136">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9a97b-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9a97b-137">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9a97b-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9a97b-138">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="9a97b-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="9a97b-139">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9a97b-139">Report Refresh Date</span></span>
- <span data-ttu-id="9a97b-140">Web</span><span class="sxs-lookup"><span data-stu-id="9a97b-140">Web</span></span>
- <span data-ttu-id="9a97b-141">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="9a97b-141">Windows Phone</span></span>
- <span data-ttu-id="9a97b-142">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="9a97b-142">Android Phone</span></span>
- <span data-ttu-id="9a97b-143">iOS</span><span class="sxs-lookup"><span data-stu-id="9a97b-143">iOS</span></span>
- <span data-ttu-id="9a97b-144">Mac</span><span class="sxs-lookup"><span data-stu-id="9a97b-144">Mac</span></span>
- <span data-ttu-id="9a97b-145">Windows</span><span class="sxs-lookup"><span data-stu-id="9a97b-145">Windows</span></span>
- <span data-ttu-id="9a97b-146">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9a97b-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9a97b-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a97b-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9a97b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a97b-148">Request</span></span>

<span data-ttu-id="9a97b-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a97b-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9a97b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a97b-150">Response</span></span>

<span data-ttu-id="9a97b-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a97b-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9a97b-152">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="9a97b-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9a97b-153">C#</span><span class="sxs-lookup"><span data-stu-id="9a97b-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a97b-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a97b-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9a97b-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9a97b-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="9a97b-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9a97b-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
