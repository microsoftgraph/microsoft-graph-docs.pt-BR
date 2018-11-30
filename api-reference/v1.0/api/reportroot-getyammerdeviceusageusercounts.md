---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
ms.openlocfilehash: 09a96ddb4ecb56dcdef9e81ef1cde6528208884d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005411"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="b4ba5-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b4ba5-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="b4ba5-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="b4ba5-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="b4ba5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ba5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4ba5-106">Permissions</span></span>

<span data-ttu-id="b4ba5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4ba5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4ba5-109">Permission type</span></span>                        | <span data-ttu-id="b4ba5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4ba5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b4ba5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4ba5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4ba5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4ba5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b4ba5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4ba5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ba5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-114">Not supported.</span></span>                           |
| <span data-ttu-id="b4ba5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4ba5-115">Application</span></span>                            | <span data-ttu-id="b4ba5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4ba5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b4ba5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ba5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b4ba5-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b4ba5-118">Function parameters</span></span>

<span data-ttu-id="b4ba5-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b4ba5-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b4ba5-120">Parameter</span></span> | <span data-ttu-id="b4ba5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4ba5-121">Type</span></span>   | <span data-ttu-id="b4ba5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4ba5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b4ba5-123">ponto</span><span class="sxs-lookup"><span data-stu-id="b4ba5-123">period</span></span>    | <span data-ttu-id="b4ba5-124">string</span><span class="sxs-lookup"><span data-stu-id="b4ba5-124">string</span></span> | <span data-ttu-id="b4ba5-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b4ba5-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b4ba5-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b4ba5-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b4ba5-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ba5-129">Request headers</span></span>

| <span data-ttu-id="b4ba5-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b4ba5-130">Name</span></span>          | <span data-ttu-id="b4ba5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4ba5-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b4ba5-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4ba5-132">Authorization</span></span> | <span data-ttu-id="b4ba5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b4ba5-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b4ba5-135">If-None-Match</span></span> | <span data-ttu-id="b4ba5-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b4ba5-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b4ba5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4ba5-138">Response</span></span>

<span data-ttu-id="b4ba5-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b4ba5-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b4ba5-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b4ba5-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b4ba5-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b4ba5-143">Report Refresh Date</span></span>
- <span data-ttu-id="b4ba5-144">Web</span><span class="sxs-lookup"><span data-stu-id="b4ba5-144">Web</span></span>
- <span data-ttu-id="b4ba5-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b4ba5-145">Windows Phone</span></span>
- <span data-ttu-id="b4ba5-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="b4ba5-146">Android Phone</span></span>
- <span data-ttu-id="b4ba5-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="b4ba5-147">iPhone</span></span>
- <span data-ttu-id="b4ba5-148">iPad</span><span class="sxs-lookup"><span data-stu-id="b4ba5-148">iPad</span></span>
- <span data-ttu-id="b4ba5-149">Outro</span><span class="sxs-lookup"><span data-stu-id="b4ba5-149">Other</span></span>
- <span data-ttu-id="b4ba5-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b4ba5-150">Report Date</span></span>
- <span data-ttu-id="b4ba5-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b4ba5-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b4ba5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4ba5-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b4ba5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4ba5-153">Request</span></span>

<span data-ttu-id="b4ba5-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b4ba5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4ba5-155">Response</span></span>

<span data-ttu-id="b4ba5-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="b4ba5-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b4ba5-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```
