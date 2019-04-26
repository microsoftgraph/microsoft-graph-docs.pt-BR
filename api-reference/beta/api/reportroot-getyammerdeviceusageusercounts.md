---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8dc72c531a5a9504384fb4c447e5841eff0b2c1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331796"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="b7401-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b7401-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7401-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7401-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="b7401-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="b7401-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7401-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7401-106">Permissions</span></span>

<span data-ttu-id="b7401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7401-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7401-109">Permission type</span></span>                        | <span data-ttu-id="b7401-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7401-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b7401-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7401-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7401-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7401-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b7401-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7401-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7401-114">Not supported.</span></span>                           |
| <span data-ttu-id="b7401-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7401-115">Application</span></span>                            | <span data-ttu-id="b7401-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7401-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b7401-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7401-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b7401-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b7401-118">Function parameters</span></span>

<span data-ttu-id="b7401-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b7401-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b7401-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b7401-120">Parameter</span></span> | <span data-ttu-id="b7401-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7401-121">Type</span></span>   | <span data-ttu-id="b7401-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7401-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b7401-123">ponto</span><span class="sxs-lookup"><span data-stu-id="b7401-123">period</span></span>    | <span data-ttu-id="b7401-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7401-124">string</span></span> | <span data-ttu-id="b7401-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b7401-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b7401-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b7401-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b7401-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b7401-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b7401-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7401-128">Required.</span></span> |

<span data-ttu-id="b7401-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7401-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b7401-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="b7401-130">The default output type is text/csv.</span></span> <span data-ttu-id="b7401-131">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b7401-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7401-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7401-132">Request headers</span></span>

| <span data-ttu-id="b7401-133">Nome</span><span class="sxs-lookup"><span data-stu-id="b7401-133">Name</span></span>          | <span data-ttu-id="b7401-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7401-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b7401-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7401-135">Authorization</span></span> | <span data-ttu-id="b7401-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7401-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b7401-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7401-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b7401-139">CSV</span><span class="sxs-lookup"><span data-stu-id="b7401-139">CSV</span></span>

<span data-ttu-id="b7401-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b7401-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b7401-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b7401-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b7401-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b7401-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b7401-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b7401-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b7401-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b7401-144">Report Refresh Date</span></span>
- <span data-ttu-id="b7401-145">Web</span><span class="sxs-lookup"><span data-stu-id="b7401-145">Web</span></span>
- <span data-ttu-id="b7401-146">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b7401-146">Windows Phone</span></span>
- <span data-ttu-id="b7401-147">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="b7401-147">Android Phone</span></span>
- <span data-ttu-id="b7401-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="b7401-148">iPhone</span></span>
- <span data-ttu-id="b7401-149">iPad</span><span class="sxs-lookup"><span data-stu-id="b7401-149">iPad</span></span>
- <span data-ttu-id="b7401-150">Outro</span><span class="sxs-lookup"><span data-stu-id="b7401-150">Other</span></span>
- <span data-ttu-id="b7401-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b7401-151">Report Date</span></span>
- <span data-ttu-id="b7401-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b7401-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b7401-153">JSON</span><span class="sxs-lookup"><span data-stu-id="b7401-153">JSON</span></span>

<span data-ttu-id="b7401-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7401-154">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7401-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7401-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b7401-156">CSV</span><span class="sxs-lookup"><span data-stu-id="b7401-156">CSV</span></span>

<span data-ttu-id="b7401-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="b7401-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b7401-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7401-158">Request</span></span>

<span data-ttu-id="b7401-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7401-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b7401-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7401-160">Response</span></span>

<span data-ttu-id="b7401-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7401-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b7401-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b7401-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b7401-163">JSON</span><span class="sxs-lookup"><span data-stu-id="b7401-163">JSON</span></span>

<span data-ttu-id="b7401-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="b7401-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b7401-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7401-165">Request</span></span>

<span data-ttu-id="b7401-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7401-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b7401-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7401-167">Response</span></span>

<span data-ttu-id="b7401-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7401-168">The following is an example of the response.</span></span>

> <span data-ttu-id="b7401-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7401-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
