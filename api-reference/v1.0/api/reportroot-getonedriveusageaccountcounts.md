---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3fecc11e17e9abdb584bef405501a6e33ca70a6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574205"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="544c6-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="544c6-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="544c6-105">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="544c6-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="544c6-106">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="544c6-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="544c6-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="544c6-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="544c6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="544c6-108">Permissions</span></span>

<span data-ttu-id="544c6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="544c6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="544c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="544c6-111">Permission type</span></span>                        | <span data-ttu-id="544c6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="544c6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="544c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="544c6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="544c6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="544c6-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="544c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="544c6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="544c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="544c6-116">Not supported.</span></span>                           |
| <span data-ttu-id="544c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="544c6-117">Application</span></span>                            | <span data-ttu-id="544c6-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="544c6-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="544c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="544c6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="544c6-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="544c6-120">Function parameters</span></span>

<span data-ttu-id="544c6-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="544c6-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="544c6-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="544c6-122">Parameter</span></span> | <span data-ttu-id="544c6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="544c6-123">Type</span></span>   | <span data-ttu-id="544c6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="544c6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="544c6-125">ponto</span><span class="sxs-lookup"><span data-stu-id="544c6-125">period</span></span>    | <span data-ttu-id="544c6-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="544c6-126">string</span></span> | <span data-ttu-id="544c6-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="544c6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="544c6-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="544c6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="544c6-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="544c6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="544c6-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="544c6-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="544c6-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="544c6-131">Request headers</span></span>

| <span data-ttu-id="544c6-132">Nome</span><span class="sxs-lookup"><span data-stu-id="544c6-132">Name</span></span>          | <span data-ttu-id="544c6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="544c6-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="544c6-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="544c6-134">Authorization</span></span> | <span data-ttu-id="544c6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="544c6-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="544c6-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="544c6-137">If-None-Match</span></span> | <span data-ttu-id="544c6-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="544c6-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="544c6-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="544c6-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="544c6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="544c6-140">Response</span></span>

<span data-ttu-id="544c6-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="544c6-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="544c6-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="544c6-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="544c6-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="544c6-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="544c6-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="544c6-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="544c6-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="544c6-145">Report Refresh Date</span></span>
- <span data-ttu-id="544c6-146">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="544c6-146">Site Type</span></span>
- <span data-ttu-id="544c6-147">Total</span><span class="sxs-lookup"><span data-stu-id="544c6-147">Total</span></span>
- <span data-ttu-id="544c6-148">Ativo</span><span class="sxs-lookup"><span data-stu-id="544c6-148">Active</span></span>
- <span data-ttu-id="544c6-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="544c6-149">Report Date</span></span>
- <span data-ttu-id="544c6-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="544c6-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="544c6-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="544c6-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="544c6-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="544c6-152">Request</span></span>

<span data-ttu-id="544c6-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="544c6-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="544c6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="544c6-154">Response</span></span>

<span data-ttu-id="544c6-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="544c6-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="544c6-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="544c6-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
