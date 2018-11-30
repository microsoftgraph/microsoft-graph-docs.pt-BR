---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
ms.openlocfilehash: a5c51bcb1dba1c4a1c15f24840ebe8923b0cc89c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005596"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="7de76-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="7de76-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="7de76-104">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="7de76-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="7de76-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="7de76-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="7de76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7de76-106">Permissions</span></span>

<span data-ttu-id="7de76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7de76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7de76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7de76-109">Permission type</span></span>                        | <span data-ttu-id="7de76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7de76-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7de76-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7de76-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7de76-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7de76-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7de76-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7de76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7de76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7de76-114">Not supported.</span></span>                           |
| <span data-ttu-id="7de76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7de76-115">Application</span></span>                            | <span data-ttu-id="7de76-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7de76-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7de76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7de76-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7de76-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7de76-118">Function parameters</span></span>

<span data-ttu-id="7de76-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7de76-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7de76-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7de76-120">Parameter</span></span> | <span data-ttu-id="7de76-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7de76-121">Type</span></span>   | <span data-ttu-id="7de76-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7de76-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7de76-123">ponto</span><span class="sxs-lookup"><span data-stu-id="7de76-123">period</span></span>    | <span data-ttu-id="7de76-124">string</span><span class="sxs-lookup"><span data-stu-id="7de76-124">string</span></span> | <span data-ttu-id="7de76-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7de76-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7de76-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7de76-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7de76-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7de76-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7de76-128">data</span><span class="sxs-lookup"><span data-stu-id="7de76-128">date</span></span>      | <span data-ttu-id="7de76-129">Data</span><span class="sxs-lookup"><span data-stu-id="7de76-129">Date</span></span>   | <span data-ttu-id="7de76-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="7de76-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7de76-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7de76-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7de76-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7de76-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7de76-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="7de76-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7de76-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7de76-134">Request headers</span></span>

| <span data-ttu-id="7de76-135">Nome</span><span class="sxs-lookup"><span data-stu-id="7de76-135">Name</span></span>          | <span data-ttu-id="7de76-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="7de76-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7de76-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="7de76-137">Authorization</span></span> | <span data-ttu-id="7de76-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7de76-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7de76-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7de76-140">If-None-Match</span></span> | <span data-ttu-id="7de76-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="7de76-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7de76-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7de76-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7de76-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de76-143">Response</span></span>

<span data-ttu-id="7de76-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7de76-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7de76-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7de76-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7de76-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7de76-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7de76-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7de76-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7de76-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7de76-148">Report Refresh Date</span></span>
- <span data-ttu-id="7de76-149">URL do site</span><span class="sxs-lookup"><span data-stu-id="7de76-149">Site URL</span></span>
- <span data-ttu-id="7de76-150">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="7de76-150">Owner Display Name</span></span>
- <span data-ttu-id="7de76-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="7de76-151">Is Deleted</span></span>
- <span data-ttu-id="7de76-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="7de76-152">Last Activity Date</span></span>
- <span data-ttu-id="7de76-153">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="7de76-153">File Count</span></span>
- <span data-ttu-id="7de76-154">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="7de76-154">Active File Count</span></span>
- <span data-ttu-id="7de76-155">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="7de76-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="7de76-156">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="7de76-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="7de76-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7de76-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7de76-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7de76-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7de76-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7de76-159">Request</span></span>

<span data-ttu-id="7de76-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7de76-160">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7de76-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de76-161">Response</span></span>

<span data-ttu-id="7de76-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7de76-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="7de76-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7de76-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```
