---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fc304242a44bd46e8127c7c2be966852484c3873
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561380"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="d16d2-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d16d2-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="d16d2-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d16d2-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="d16d2-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="d16d2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="d16d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d16d2-106">Permissions</span></span>

<span data-ttu-id="d16d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d16d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d16d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d16d2-109">Permission type</span></span>                        | <span data-ttu-id="d16d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d16d2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d16d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d16d2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d16d2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d16d2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d16d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d16d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d16d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d16d2-114">Not supported.</span></span>                           |
| <span data-ttu-id="d16d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d16d2-115">Application</span></span>                            | <span data-ttu-id="d16d2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d16d2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d16d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d16d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d16d2-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d16d2-118">Function parameters</span></span>

<span data-ttu-id="d16d2-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d16d2-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d16d2-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d16d2-120">Parameter</span></span> | <span data-ttu-id="d16d2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d16d2-121">Type</span></span>   | <span data-ttu-id="d16d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d16d2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d16d2-123">ponto</span><span class="sxs-lookup"><span data-stu-id="d16d2-123">period</span></span>    | <span data-ttu-id="d16d2-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d16d2-124">string</span></span> | <span data-ttu-id="d16d2-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d16d2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d16d2-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d16d2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d16d2-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d16d2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d16d2-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d16d2-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d16d2-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d16d2-129">Request headers</span></span>

| <span data-ttu-id="d16d2-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d16d2-130">Name</span></span>          | <span data-ttu-id="d16d2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d16d2-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d16d2-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d16d2-132">Authorization</span></span> | <span data-ttu-id="d16d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d16d2-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d16d2-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d16d2-135">If-None-Match</span></span> | <span data-ttu-id="d16d2-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d16d2-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d16d2-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d16d2-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d16d2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d16d2-138">Response</span></span>

<span data-ttu-id="d16d2-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d16d2-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d16d2-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d16d2-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d16d2-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d16d2-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d16d2-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d16d2-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d16d2-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d16d2-143">Report Refresh Date</span></span>
- <span data-ttu-id="d16d2-144">Web</span><span class="sxs-lookup"><span data-stu-id="d16d2-144">Web</span></span>
- <span data-ttu-id="d16d2-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d16d2-145">Windows Phone</span></span>
- <span data-ttu-id="d16d2-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="d16d2-146">Android Phone</span></span>
- <span data-ttu-id="d16d2-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="d16d2-147">iPhone</span></span>
- <span data-ttu-id="d16d2-148">iPad</span><span class="sxs-lookup"><span data-stu-id="d16d2-148">iPad</span></span>
- <span data-ttu-id="d16d2-149">Outro</span><span class="sxs-lookup"><span data-stu-id="d16d2-149">Other</span></span>
- <span data-ttu-id="d16d2-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d16d2-150">Report Date</span></span>
- <span data-ttu-id="d16d2-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d16d2-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d16d2-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d16d2-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d16d2-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d16d2-153">Request</span></span>

<span data-ttu-id="d16d2-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d16d2-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d16d2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d16d2-155">Response</span></span>

<span data-ttu-id="d16d2-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d16d2-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="d16d2-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d16d2-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```
