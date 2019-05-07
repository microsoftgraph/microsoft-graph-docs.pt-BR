---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5c5ddb888eb1db466642269b4b82f6e147ab8a42
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603738"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="d914d-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d914d-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="d914d-104">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d914d-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="d914d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="d914d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="d914d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d914d-106">Permissions</span></span>

<span data-ttu-id="d914d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d914d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d914d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d914d-109">Permission type</span></span>                        | <span data-ttu-id="d914d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d914d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d914d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d914d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d914d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d914d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d914d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d914d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d914d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d914d-114">Not supported.</span></span>                           |
| <span data-ttu-id="d914d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d914d-115">Application</span></span>                            | <span data-ttu-id="d914d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d914d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d914d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d914d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d914d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d914d-118">Function parameters</span></span>

<span data-ttu-id="d914d-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d914d-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d914d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d914d-120">Parameter</span></span> | <span data-ttu-id="d914d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d914d-121">Type</span></span>   | <span data-ttu-id="d914d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d914d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d914d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="d914d-123">period</span></span>    | <span data-ttu-id="d914d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d914d-124">string</span></span> | <span data-ttu-id="d914d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d914d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d914d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d914d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d914d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d914d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d914d-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d914d-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d914d-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d914d-129">Request headers</span></span>

| <span data-ttu-id="d914d-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d914d-130">Name</span></span>          | <span data-ttu-id="d914d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d914d-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d914d-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d914d-132">Authorization</span></span> | <span data-ttu-id="d914d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d914d-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d914d-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d914d-135">If-None-Match</span></span> | <span data-ttu-id="d914d-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d914d-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d914d-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d914d-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d914d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d914d-138">Response</span></span>

<span data-ttu-id="d914d-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d914d-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d914d-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d914d-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d914d-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d914d-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d914d-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d914d-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d914d-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d914d-143">Report Refresh Date</span></span>
- <span data-ttu-id="d914d-144">Web</span><span class="sxs-lookup"><span data-stu-id="d914d-144">Web</span></span>
- <span data-ttu-id="d914d-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d914d-145">Windows Phone</span></span>
- <span data-ttu-id="d914d-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="d914d-146">Android Phone</span></span>
- <span data-ttu-id="d914d-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="d914d-147">iPhone</span></span>
- <span data-ttu-id="d914d-148">iPad</span><span class="sxs-lookup"><span data-stu-id="d914d-148">iPad</span></span>
- <span data-ttu-id="d914d-149">Outro</span><span class="sxs-lookup"><span data-stu-id="d914d-149">Other</span></span>
- <span data-ttu-id="d914d-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d914d-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d914d-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d914d-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d914d-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d914d-152">Request</span></span>

<span data-ttu-id="d914d-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d914d-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d914d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d914d-154">Response</span></span>

<span data-ttu-id="d914d-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d914d-155">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d914d-156">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d914d-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d914d-157">Basic</span><span class="sxs-lookup"><span data-stu-id="d914d-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusagedistributionusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d914d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d914d-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusagedistributionusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d914d-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d914d-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
