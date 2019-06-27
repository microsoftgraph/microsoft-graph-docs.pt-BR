---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Obtenha dados sobre o uso do dispositivo Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 35d4bdebcdd6b6d9fe25093bf9f50946a5552538
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271769"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="49902-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="49902-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="49902-104">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="49902-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="49902-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="49902-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="49902-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49902-106">Permissions</span></span>

<span data-ttu-id="49902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49902-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49902-109">Permission type</span></span>                        | <span data-ttu-id="49902-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49902-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="49902-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49902-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49902-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="49902-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="49902-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49902-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49902-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49902-114">Not supported.</span></span>                           |
| <span data-ttu-id="49902-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49902-115">Application</span></span>                            | <span data-ttu-id="49902-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="49902-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="49902-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49902-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="49902-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="49902-118">Function parameters</span></span>

<span data-ttu-id="49902-119">Na URL da solicitação, forneça um valor válido ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="49902-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="49902-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="49902-120">Parameter</span></span> | <span data-ttu-id="49902-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="49902-121">Type</span></span>   | <span data-ttu-id="49902-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="49902-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="49902-123">ponto</span><span class="sxs-lookup"><span data-stu-id="49902-123">period</span></span>    | <span data-ttu-id="49902-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49902-124">string</span></span> | <span data-ttu-id="49902-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="49902-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="49902-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="49902-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="49902-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="49902-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="49902-128">data</span><span class="sxs-lookup"><span data-stu-id="49902-128">date</span></span>      | <span data-ttu-id="49902-129">Data</span><span class="sxs-lookup"><span data-stu-id="49902-129">Date</span></span>   | <span data-ttu-id="49902-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="49902-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="49902-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="49902-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="49902-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="49902-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="49902-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="49902-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49902-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49902-134">Request headers</span></span>

| <span data-ttu-id="49902-135">Nome</span><span class="sxs-lookup"><span data-stu-id="49902-135">Name</span></span>          | <span data-ttu-id="49902-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="49902-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="49902-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="49902-137">Authorization</span></span> | <span data-ttu-id="49902-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49902-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="49902-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="49902-140">If-None-Match</span></span> | <span data-ttu-id="49902-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="49902-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="49902-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="49902-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="49902-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="49902-143">Response</span></span>

<span data-ttu-id="49902-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="49902-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="49902-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="49902-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="49902-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="49902-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="49902-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="49902-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="49902-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="49902-148">Report Refresh Date</span></span>
- <span data-ttu-id="49902-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="49902-149">User Principal Name</span></span>
- <span data-ttu-id="49902-150">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="49902-150">Display Name</span></span>
- <span data-ttu-id="49902-151">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="49902-151">User State</span></span>
- <span data-ttu-id="49902-152">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="49902-152">State Change Date</span></span>
- <span data-ttu-id="49902-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="49902-153">Last Activity Date</span></span>
- <span data-ttu-id="49902-154">Usou Web</span><span class="sxs-lookup"><span data-stu-id="49902-154">Used Web</span></span>
- <span data-ttu-id="49902-155">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="49902-155">Used Windows Phone</span></span>
- <span data-ttu-id="49902-156">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="49902-156">Used Android Phone</span></span>
- <span data-ttu-id="49902-157">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="49902-157">Used iPhone</span></span>
- <span data-ttu-id="49902-158">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="49902-158">Used iPad</span></span>
- <span data-ttu-id="49902-159">Usou outros</span><span class="sxs-lookup"><span data-stu-id="49902-159">Used Others</span></span>
- <span data-ttu-id="49902-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="49902-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="49902-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49902-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="49902-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49902-162">Request</span></span>

<span data-ttu-id="49902-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49902-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="49902-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="49902-164">Response</span></span>

<span data-ttu-id="49902-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49902-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="49902-166">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="49902-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="49902-167">C#</span><span class="sxs-lookup"><span data-stu-id="49902-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49902-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="49902-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="49902-169">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="49902-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request"></a><span data-ttu-id="49902-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49902-170">Request</span></span>

<span data-ttu-id="49902-171">Se chamado com o `date` parâmetro, o relatório terá o escopo para uso na data especificada.</span><span class="sxs-lookup"><span data-stu-id="49902-171">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="49902-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="49902-172">Response</span></span>

<span data-ttu-id="49902-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49902-173">The following is an example of the response.</span></span>

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

<span data-ttu-id="49902-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="49902-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
