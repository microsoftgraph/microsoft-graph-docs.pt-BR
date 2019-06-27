---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6fa19922b928e1d743b69869110ba96ce4a82b56
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276234"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="3cc93-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="3cc93-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="3cc93-105">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="3cc93-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="3cc93-106">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="3cc93-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="3cc93-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="3cc93-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="3cc93-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cc93-108">Permissions</span></span>

<span data-ttu-id="3cc93-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cc93-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cc93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cc93-111">Permission type</span></span>                        | <span data-ttu-id="3cc93-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cc93-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3cc93-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cc93-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cc93-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cc93-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3cc93-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cc93-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cc93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc93-116">Not supported.</span></span>                           |
| <span data-ttu-id="3cc93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cc93-117">Application</span></span>                            | <span data-ttu-id="3cc93-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cc93-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3cc93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc93-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3cc93-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3cc93-120">Function parameters</span></span>

<span data-ttu-id="3cc93-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3cc93-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3cc93-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3cc93-122">Parameter</span></span> | <span data-ttu-id="3cc93-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cc93-123">Type</span></span>   | <span data-ttu-id="3cc93-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc93-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3cc93-125">ponto</span><span class="sxs-lookup"><span data-stu-id="3cc93-125">period</span></span>    | <span data-ttu-id="3cc93-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cc93-126">string</span></span> | <span data-ttu-id="3cc93-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3cc93-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3cc93-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3cc93-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3cc93-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3cc93-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3cc93-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cc93-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3cc93-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc93-131">Request headers</span></span>

| <span data-ttu-id="3cc93-132">Nome</span><span class="sxs-lookup"><span data-stu-id="3cc93-132">Name</span></span>          | <span data-ttu-id="3cc93-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc93-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3cc93-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cc93-134">Authorization</span></span> | <span data-ttu-id="3cc93-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cc93-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3cc93-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3cc93-137">If-None-Match</span></span> | <span data-ttu-id="3cc93-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3cc93-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3cc93-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3cc93-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3cc93-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc93-140">Response</span></span>

<span data-ttu-id="3cc93-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3cc93-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3cc93-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc93-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3cc93-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3cc93-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3cc93-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3cc93-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3cc93-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3cc93-145">Report Refresh Date</span></span>
- <span data-ttu-id="3cc93-146">Windows</span><span class="sxs-lookup"><span data-stu-id="3cc93-146">Windows</span></span>
- <span data-ttu-id="3cc93-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="3cc93-147">Windows Phone</span></span>
- <span data-ttu-id="3cc93-148">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="3cc93-148">Android Phone</span></span>
- <span data-ttu-id="3cc93-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="3cc93-149">iPhone</span></span>
- <span data-ttu-id="3cc93-150">iPad</span><span class="sxs-lookup"><span data-stu-id="3cc93-150">iPad</span></span>
- <span data-ttu-id="3cc93-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3cc93-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3cc93-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cc93-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3cc93-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc93-153">Request</span></span>

<span data-ttu-id="3cc93-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cc93-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3cc93-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc93-155">Response</span></span>

<span data-ttu-id="3cc93-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc93-156">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3cc93-157">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="3cc93-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3cc93-158">C#</span><span class="sxs-lookup"><span data-stu-id="3cc93-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cc93-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cc93-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3cc93-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cc93-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="3cc93-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3cc93-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
