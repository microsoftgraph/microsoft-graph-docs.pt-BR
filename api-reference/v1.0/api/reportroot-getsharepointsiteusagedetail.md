---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Obtenha dados sobre o uso do site do SharePoint.
ms.openlocfilehash: 3946aa8d6e60368d5fde39ec7c487a14dd678013
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005176"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="e8d53-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="e8d53-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="e8d53-104">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e8d53-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="e8d53-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="e8d53-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d53-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8d53-106">Permissions</span></span>

<span data-ttu-id="e8d53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8d53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8d53-109">Permission type</span></span>                        | <span data-ttu-id="e8d53-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8d53-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e8d53-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8d53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8d53-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8d53-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e8d53-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8d53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d53-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8d53-114">Not supported.</span></span>                           |
| <span data-ttu-id="e8d53-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8d53-115">Application</span></span>                            | <span data-ttu-id="e8d53-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8d53-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e8d53-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d53-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e8d53-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e8d53-118">Function parameters</span></span>

<span data-ttu-id="e8d53-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e8d53-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e8d53-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e8d53-120">Parameter</span></span> | <span data-ttu-id="e8d53-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8d53-121">Type</span></span>   | <span data-ttu-id="e8d53-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d53-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e8d53-123">ponto</span><span class="sxs-lookup"><span data-stu-id="e8d53-123">period</span></span>    | <span data-ttu-id="e8d53-124">string</span><span class="sxs-lookup"><span data-stu-id="e8d53-124">string</span></span> | <span data-ttu-id="e8d53-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e8d53-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e8d53-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e8d53-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e8d53-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e8d53-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e8d53-128">data</span><span class="sxs-lookup"><span data-stu-id="e8d53-128">date</span></span>      | <span data-ttu-id="e8d53-129">Data</span><span class="sxs-lookup"><span data-stu-id="e8d53-129">Date</span></span>   | <span data-ttu-id="e8d53-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="e8d53-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e8d53-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="e8d53-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e8d53-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e8d53-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e8d53-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="e8d53-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8d53-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d53-134">Request headers</span></span>

| <span data-ttu-id="e8d53-135">Nome</span><span class="sxs-lookup"><span data-stu-id="e8d53-135">Name</span></span>          | <span data-ttu-id="e8d53-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d53-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e8d53-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8d53-137">Authorization</span></span> | <span data-ttu-id="e8d53-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8d53-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e8d53-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e8d53-140">If-None-Match</span></span> | <span data-ttu-id="e8d53-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="e8d53-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e8d53-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e8d53-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e8d53-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d53-143">Response</span></span>

<span data-ttu-id="e8d53-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e8d53-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e8d53-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d53-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e8d53-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e8d53-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e8d53-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e8d53-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e8d53-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e8d53-148">Report Refresh Date</span></span>
- <span data-ttu-id="e8d53-149">Id do site</span><span class="sxs-lookup"><span data-stu-id="e8d53-149">Site Id</span></span>
- <span data-ttu-id="e8d53-150">URL do site</span><span class="sxs-lookup"><span data-stu-id="e8d53-150">Site URL</span></span>
- <span data-ttu-id="e8d53-151">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="e8d53-151">Owner Display Name</span></span>
- <span data-ttu-id="e8d53-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="e8d53-152">Is Deleted</span></span>
- <span data-ttu-id="e8d53-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="e8d53-153">Last Activity Date</span></span>
- <span data-ttu-id="e8d53-154">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="e8d53-154">File Count</span></span>
- <span data-ttu-id="e8d53-155">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="e8d53-155">Active File Count</span></span>
- <span data-ttu-id="e8d53-156">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="e8d53-156">Page View Count</span></span>
- <span data-ttu-id="e8d53-157">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="e8d53-157">Visited Page Count</span></span>
- <span data-ttu-id="e8d53-158">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="e8d53-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="e8d53-159">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="e8d53-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="e8d53-160">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="e8d53-160">Root Web Template</span></span>
- <span data-ttu-id="e8d53-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e8d53-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e8d53-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8d53-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e8d53-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d53-163">Request</span></span>

<span data-ttu-id="e8d53-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8d53-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e8d53-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d53-165">Response</span></span>

<span data-ttu-id="e8d53-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d53-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="e8d53-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e8d53-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```
