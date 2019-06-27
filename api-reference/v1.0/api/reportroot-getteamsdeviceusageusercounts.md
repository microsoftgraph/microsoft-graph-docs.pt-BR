---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 907a9b88afc254999a9eda242adbf3c1a896fe51
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277172"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="6de65-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="6de65-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="6de65-104">Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6de65-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6de65-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6de65-105">Permissions</span></span>

<span data-ttu-id="6de65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6de65-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6de65-108">Permission type</span></span>                        | <span data-ttu-id="6de65-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6de65-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6de65-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6de65-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6de65-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6de65-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6de65-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6de65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6de65-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6de65-113">Not supported.</span></span>                           |
| <span data-ttu-id="6de65-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6de65-114">Application</span></span>                            | <span data-ttu-id="6de65-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6de65-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6de65-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6de65-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6de65-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6de65-117">Function parameters</span></span>

<span data-ttu-id="6de65-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6de65-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6de65-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6de65-119">Parameter</span></span> | <span data-ttu-id="6de65-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6de65-120">Type</span></span>   | <span data-ttu-id="6de65-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6de65-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6de65-122">ponto</span><span class="sxs-lookup"><span data-stu-id="6de65-122">period</span></span>    | <span data-ttu-id="6de65-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6de65-123">string</span></span> | <span data-ttu-id="6de65-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6de65-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6de65-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6de65-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6de65-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6de65-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6de65-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6de65-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6de65-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6de65-128">Request headers</span></span>

| <span data-ttu-id="6de65-129">Nome</span><span class="sxs-lookup"><span data-stu-id="6de65-129">Name</span></span>          | <span data-ttu-id="6de65-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6de65-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6de65-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="6de65-131">Authorization</span></span> | <span data-ttu-id="6de65-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6de65-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6de65-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6de65-134">Response</span></span>

<span data-ttu-id="6de65-135">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6de65-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6de65-136">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6de65-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6de65-137">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6de65-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6de65-138">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="6de65-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="6de65-139">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6de65-139">Report Refresh Date</span></span>
- <span data-ttu-id="6de65-140">Web</span><span class="sxs-lookup"><span data-stu-id="6de65-140">Web</span></span>
- <span data-ttu-id="6de65-141">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="6de65-141">Windows Phone</span></span>
- <span data-ttu-id="6de65-142">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="6de65-142">Android Phone</span></span>
- <span data-ttu-id="6de65-143">iOS</span><span class="sxs-lookup"><span data-stu-id="6de65-143">iOS</span></span>
- <span data-ttu-id="6de65-144">Mac</span><span class="sxs-lookup"><span data-stu-id="6de65-144">Mac</span></span>
- <span data-ttu-id="6de65-145">Windows</span><span class="sxs-lookup"><span data-stu-id="6de65-145">Windows</span></span>
- <span data-ttu-id="6de65-146">Data do Relatório</span><span class="sxs-lookup"><span data-stu-id="6de65-146">Report Date</span></span>
- <span data-ttu-id="6de65-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6de65-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6de65-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6de65-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6de65-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6de65-149">Request</span></span>

<span data-ttu-id="6de65-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6de65-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6de65-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6de65-151">Response</span></span>

<span data-ttu-id="6de65-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6de65-152">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6de65-153">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="6de65-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6de65-154">C#</span><span class="sxs-lookup"><span data-stu-id="6de65-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6de65-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="6de65-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6de65-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6de65-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6de65-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6de65-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
