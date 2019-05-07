---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 69f149d408e047d10727c6a334c910faf6031e0c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603415"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="d3e23-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d3e23-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="d3e23-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3e23-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="d3e23-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="d3e23-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3e23-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3e23-106">Permissions</span></span>

<span data-ttu-id="d3e23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3e23-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3e23-109">Permission type</span></span>                        | <span data-ttu-id="d3e23-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3e23-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d3e23-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3e23-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3e23-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3e23-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d3e23-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3e23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3e23-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e23-114">Not supported.</span></span>                           |
| <span data-ttu-id="d3e23-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3e23-115">Application</span></span>                            | <span data-ttu-id="d3e23-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3e23-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d3e23-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e23-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d3e23-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d3e23-118">Function parameters</span></span>

<span data-ttu-id="d3e23-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d3e23-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d3e23-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3e23-120">Parameter</span></span> | <span data-ttu-id="d3e23-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3e23-121">Type</span></span>   | <span data-ttu-id="d3e23-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e23-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d3e23-123">ponto</span><span class="sxs-lookup"><span data-stu-id="d3e23-123">period</span></span>    | <span data-ttu-id="d3e23-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3e23-124">string</span></span> | <span data-ttu-id="d3e23-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d3e23-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d3e23-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d3e23-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d3e23-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d3e23-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d3e23-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e23-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d3e23-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e23-129">Request headers</span></span>

| <span data-ttu-id="d3e23-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d3e23-130">Name</span></span>          | <span data-ttu-id="d3e23-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e23-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d3e23-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3e23-132">Authorization</span></span> | <span data-ttu-id="d3e23-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e23-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d3e23-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d3e23-135">If-None-Match</span></span> | <span data-ttu-id="d3e23-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d3e23-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d3e23-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3e23-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d3e23-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e23-138">Response</span></span>

<span data-ttu-id="d3e23-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d3e23-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d3e23-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e23-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d3e23-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d3e23-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d3e23-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d3e23-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d3e23-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d3e23-143">Report Refresh Date</span></span>
- <span data-ttu-id="d3e23-144">Web</span><span class="sxs-lookup"><span data-stu-id="d3e23-144">Web</span></span>
- <span data-ttu-id="d3e23-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d3e23-145">Windows Phone</span></span>
- <span data-ttu-id="d3e23-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="d3e23-146">Android Phone</span></span>
- <span data-ttu-id="d3e23-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="d3e23-147">iPhone</span></span>
- <span data-ttu-id="d3e23-148">iPad</span><span class="sxs-lookup"><span data-stu-id="d3e23-148">iPad</span></span>
- <span data-ttu-id="d3e23-149">Outro</span><span class="sxs-lookup"><span data-stu-id="d3e23-149">Other</span></span>
- <span data-ttu-id="d3e23-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d3e23-150">Report Date</span></span>
- <span data-ttu-id="d3e23-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d3e23-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d3e23-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3e23-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3e23-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e23-153">Request</span></span>

<span data-ttu-id="d3e23-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e23-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d3e23-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e23-155">Response</span></span>

<span data-ttu-id="d3e23-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e23-156">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3e23-157">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d3e23-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3e23-158">Basic</span><span class="sxs-lookup"><span data-stu-id="d3e23-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3e23-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3e23-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d3e23-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d3e23-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
