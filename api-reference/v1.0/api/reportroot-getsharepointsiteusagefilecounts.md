---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2dff4b45f76c82ef15552078c854c5f23bdeff21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970975"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="c0f37-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="c0f37-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

<span data-ttu-id="c0f37-105">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="c0f37-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="c0f37-106">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c0f37-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="c0f37-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="c0f37-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0f37-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0f37-108">Permissions</span></span>

<span data-ttu-id="c0f37-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f37-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0f37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0f37-111">Permission type</span></span>                        | <span data-ttu-id="c0f37-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0f37-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c0f37-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0f37-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0f37-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f37-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c0f37-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0f37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f37-116">Not supported.</span></span>                           |
| <span data-ttu-id="c0f37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0f37-117">Application</span></span>                            | <span data-ttu-id="c0f37-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f37-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c0f37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f37-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c0f37-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c0f37-120">Function parameters</span></span>

<span data-ttu-id="c0f37-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c0f37-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c0f37-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c0f37-122">Parameter</span></span> | <span data-ttu-id="c0f37-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0f37-123">Type</span></span>   | <span data-ttu-id="c0f37-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f37-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c0f37-125">ponto</span><span class="sxs-lookup"><span data-stu-id="c0f37-125">period</span></span>    | <span data-ttu-id="c0f37-126">string</span><span class="sxs-lookup"><span data-stu-id="c0f37-126">string</span></span> | <span data-ttu-id="c0f37-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c0f37-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c0f37-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c0f37-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c0f37-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c0f37-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c0f37-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0f37-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c0f37-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f37-131">Request headers</span></span>

| <span data-ttu-id="c0f37-132">Nome</span><span class="sxs-lookup"><span data-stu-id="c0f37-132">Name</span></span>          | <span data-ttu-id="c0f37-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f37-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c0f37-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0f37-134">Authorization</span></span> | <span data-ttu-id="c0f37-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0f37-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c0f37-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c0f37-137">If-None-Match</span></span> | <span data-ttu-id="c0f37-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="c0f37-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c0f37-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0f37-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c0f37-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f37-140">Response</span></span>

<span data-ttu-id="c0f37-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c0f37-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c0f37-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f37-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c0f37-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c0f37-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c0f37-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c0f37-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c0f37-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c0f37-145">Report Refresh Date</span></span>
- <span data-ttu-id="c0f37-146">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="c0f37-146">Site Type</span></span>
- <span data-ttu-id="c0f37-147">Total</span><span class="sxs-lookup"><span data-stu-id="c0f37-147">Total</span></span>
- <span data-ttu-id="c0f37-148">Ativo</span><span class="sxs-lookup"><span data-stu-id="c0f37-148">Active</span></span>
- <span data-ttu-id="c0f37-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="c0f37-149">Report Date</span></span>
- <span data-ttu-id="c0f37-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c0f37-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c0f37-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0f37-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c0f37-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f37-152">Request</span></span>

<span data-ttu-id="c0f37-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0f37-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c0f37-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f37-154">Response</span></span>

<span data-ttu-id="c0f37-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f37-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="c0f37-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c0f37-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
