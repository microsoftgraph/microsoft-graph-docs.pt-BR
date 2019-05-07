---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b9d3560860fef2be062d1609bdba2644b8ef410e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604612"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="59eb7-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="59eb7-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="59eb7-105">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="59eb7-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="59eb7-106">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="59eb7-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="59eb7-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="59eb7-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="59eb7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="59eb7-108">Permissions</span></span>

<span data-ttu-id="59eb7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59eb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59eb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59eb7-111">Permission type</span></span>                        | <span data-ttu-id="59eb7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59eb7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="59eb7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59eb7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="59eb7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59eb7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="59eb7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59eb7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59eb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59eb7-116">Not supported.</span></span>                           |
| <span data-ttu-id="59eb7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59eb7-117">Application</span></span>                            | <span data-ttu-id="59eb7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59eb7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="59eb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59eb7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="59eb7-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="59eb7-120">Function parameters</span></span>

<span data-ttu-id="59eb7-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="59eb7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="59eb7-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59eb7-122">Parameter</span></span> | <span data-ttu-id="59eb7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="59eb7-123">Type</span></span>   | <span data-ttu-id="59eb7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="59eb7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="59eb7-125">ponto</span><span class="sxs-lookup"><span data-stu-id="59eb7-125">period</span></span>    | <span data-ttu-id="59eb7-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59eb7-126">string</span></span> | <span data-ttu-id="59eb7-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="59eb7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="59eb7-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="59eb7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="59eb7-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="59eb7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="59eb7-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59eb7-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="59eb7-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59eb7-131">Request headers</span></span>

| <span data-ttu-id="59eb7-132">Nome</span><span class="sxs-lookup"><span data-stu-id="59eb7-132">Name</span></span>          | <span data-ttu-id="59eb7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="59eb7-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="59eb7-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="59eb7-134">Authorization</span></span> | <span data-ttu-id="59eb7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59eb7-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="59eb7-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="59eb7-137">If-None-Match</span></span> | <span data-ttu-id="59eb7-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="59eb7-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="59eb7-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59eb7-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="59eb7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="59eb7-140">Response</span></span>

<span data-ttu-id="59eb7-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="59eb7-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="59eb7-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="59eb7-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="59eb7-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="59eb7-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="59eb7-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="59eb7-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="59eb7-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="59eb7-145">Report Refresh Date</span></span>
- <span data-ttu-id="59eb7-146">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="59eb7-146">Site Type</span></span>
- <span data-ttu-id="59eb7-147">Total</span><span class="sxs-lookup"><span data-stu-id="59eb7-147">Total</span></span>
- <span data-ttu-id="59eb7-148">Ativo</span><span class="sxs-lookup"><span data-stu-id="59eb7-148">Active</span></span>
- <span data-ttu-id="59eb7-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="59eb7-149">Report Date</span></span>
- <span data-ttu-id="59eb7-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="59eb7-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="59eb7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59eb7-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="59eb7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59eb7-152">Request</span></span>

<span data-ttu-id="59eb7-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59eb7-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="59eb7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="59eb7-154">Response</span></span>

<span data-ttu-id="59eb7-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59eb7-155">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="59eb7-156">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="59eb7-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="59eb7-157">Basic</span><span class="sxs-lookup"><span data-stu-id="59eb7-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagesitecounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59eb7-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59eb7-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagesitecounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="59eb7-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="59eb7-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getsharepointsiteusagesitecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointsiteusagesitecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
