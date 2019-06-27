---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 91502db719dc25d72a4a613eb56bbce6e4f0abc1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276185"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="cde4e-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="cde4e-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="cde4e-105">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="cde4e-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="cde4e-106">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cde4e-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="cde4e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="cde4e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="cde4e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cde4e-108">Permissions</span></span>

<span data-ttu-id="cde4e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cde4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cde4e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cde4e-111">Permission type</span></span>                        | <span data-ttu-id="cde4e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cde4e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cde4e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cde4e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cde4e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cde4e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cde4e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cde4e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde4e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde4e-116">Not supported.</span></span>                           |
| <span data-ttu-id="cde4e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cde4e-117">Application</span></span>                            | <span data-ttu-id="cde4e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cde4e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cde4e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cde4e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cde4e-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cde4e-120">Function parameters</span></span>

<span data-ttu-id="cde4e-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="cde4e-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cde4e-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cde4e-122">Parameter</span></span> | <span data-ttu-id="cde4e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cde4e-123">Type</span></span>   | <span data-ttu-id="cde4e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cde4e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cde4e-125">ponto</span><span class="sxs-lookup"><span data-stu-id="cde4e-125">period</span></span>    | <span data-ttu-id="cde4e-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cde4e-126">string</span></span> | <span data-ttu-id="cde4e-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cde4e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cde4e-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="cde4e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cde4e-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cde4e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cde4e-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cde4e-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cde4e-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cde4e-131">Request headers</span></span>

| <span data-ttu-id="cde4e-132">Nome</span><span class="sxs-lookup"><span data-stu-id="cde4e-132">Name</span></span>          | <span data-ttu-id="cde4e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cde4e-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="cde4e-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="cde4e-134">Authorization</span></span> | <span data-ttu-id="cde4e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cde4e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="cde4e-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cde4e-137">If-None-Match</span></span> | <span data-ttu-id="cde4e-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="cde4e-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="cde4e-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cde4e-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cde4e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cde4e-140">Response</span></span>

<span data-ttu-id="cde4e-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="cde4e-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cde4e-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="cde4e-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cde4e-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cde4e-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cde4e-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="cde4e-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cde4e-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="cde4e-145">Report Refresh Date</span></span>
- <span data-ttu-id="cde4e-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="cde4e-146">Report Date</span></span>
- <span data-ttu-id="cde4e-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="cde4e-147">Report Period</span></span>
- <span data-ttu-id="cde4e-148">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="cde4e-148">Audio/Video</span></span>
- <span data-ttu-id="cde4e-149">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="cde4e-149">Dial-in Microsoft</span></span>
- <span data-ttu-id="cde4e-150">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="cde4e-150">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="cde4e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cde4e-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cde4e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cde4e-152">Request</span></span>

<span data-ttu-id="cde4e-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cde4e-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="cde4e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="cde4e-154">Response</span></span>

<span data-ttu-id="cde4e-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cde4e-155">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cde4e-156">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="cde4e-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cde4e-157">C#</span><span class="sxs-lookup"><span data-stu-id="cde4e-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cde4e-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="cde4e-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cde4e-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cde4e-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="cde4e-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="cde4e-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
