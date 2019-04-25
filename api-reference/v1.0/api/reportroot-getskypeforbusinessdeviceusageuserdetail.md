---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bf4fb6da750b54d220ca6d7319132ff62b3661f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574184"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="5f1b2-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5f1b2-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="5f1b2-104">Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="5f1b2-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="5f1b2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f1b2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f1b2-106">Permissions</span></span>

<span data-ttu-id="5f1b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f1b2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f1b2-109">Permission type</span></span>                        | <span data-ttu-id="5f1b2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f1b2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5f1b2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f1b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f1b2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f1b2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5f1b2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f1b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f1b2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-114">Not supported.</span></span>                           |
| <span data-ttu-id="5f1b2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f1b2-115">Application</span></span>                            | <span data-ttu-id="5f1b2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f1b2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5f1b2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1b2-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5f1b2-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5f1b2-118">Function parameters</span></span>

<span data-ttu-id="5f1b2-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5f1b2-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f1b2-120">Parameter</span></span> | <span data-ttu-id="5f1b2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f1b2-121">Type</span></span>   | <span data-ttu-id="5f1b2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f1b2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5f1b2-123">ponto</span><span class="sxs-lookup"><span data-stu-id="5f1b2-123">period</span></span>    | <span data-ttu-id="5f1b2-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f1b2-124">string</span></span> | <span data-ttu-id="5f1b2-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5f1b2-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5f1b2-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5f1b2-128">data</span><span class="sxs-lookup"><span data-stu-id="5f1b2-128">date</span></span>      | <span data-ttu-id="5f1b2-129">Data</span><span class="sxs-lookup"><span data-stu-id="5f1b2-129">Date</span></span>   | <span data-ttu-id="5f1b2-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5f1b2-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5f1b2-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5f1b2-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f1b2-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1b2-134">Request headers</span></span>

| <span data-ttu-id="5f1b2-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5f1b2-135">Name</span></span>          | <span data-ttu-id="5f1b2-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f1b2-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5f1b2-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f1b2-137">Authorization</span></span> | <span data-ttu-id="5f1b2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5f1b2-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5f1b2-140">If-None-Match</span></span> | <span data-ttu-id="5f1b2-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5f1b2-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5f1b2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1b2-143">Response</span></span>

<span data-ttu-id="5f1b2-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5f1b2-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5f1b2-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5f1b2-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5f1b2-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5f1b2-148">Report Refresh Date</span></span>
- <span data-ttu-id="5f1b2-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="5f1b2-149">User Principal Name</span></span>
- <span data-ttu-id="5f1b2-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="5f1b2-150">Last Activity Date</span></span>
- <span data-ttu-id="5f1b2-151">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="5f1b2-151">Used Windows</span></span>
- <span data-ttu-id="5f1b2-152">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5f1b2-152">Used Windows Phone</span></span>
- <span data-ttu-id="5f1b2-153">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="5f1b2-153">Used Android Phone</span></span>
- <span data-ttu-id="5f1b2-154">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="5f1b2-154">Used iPhone</span></span>
- <span data-ttu-id="5f1b2-155">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="5f1b2-155">Used iPad</span></span>
- <span data-ttu-id="5f1b2-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5f1b2-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5f1b2-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f1b2-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f1b2-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1b2-158">Request</span></span>

<span data-ttu-id="5f1b2-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5f1b2-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1b2-160">Response</span></span>

<span data-ttu-id="5f1b2-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="5f1b2-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5f1b2-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```
