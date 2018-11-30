---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
ms.openlocfilehash: 55b502ae31a2219e745ad32a2946393d091a30af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035068"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="577df-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="577df-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

> <span data-ttu-id="577df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="577df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="577df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="577df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="577df-106">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="577df-106">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="577df-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="577df-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="577df-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="577df-108">Permissions</span></span>

<span data-ttu-id="577df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="577df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="577df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="577df-111">Permission type</span></span>                        | <span data-ttu-id="577df-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="577df-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="577df-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="577df-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="577df-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="577df-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="577df-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="577df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="577df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="577df-116">Not supported.</span></span>                           |
| <span data-ttu-id="577df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="577df-117">Application</span></span>                            | <span data-ttu-id="577df-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="577df-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="577df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="577df-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="577df-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="577df-120">Function parameters</span></span>

<span data-ttu-id="577df-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="577df-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="577df-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="577df-122">Parameter</span></span> | <span data-ttu-id="577df-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="577df-123">Type</span></span>   | <span data-ttu-id="577df-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="577df-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="577df-125">ponto</span><span class="sxs-lookup"><span data-stu-id="577df-125">period</span></span>    | <span data-ttu-id="577df-126">string</span><span class="sxs-lookup"><span data-stu-id="577df-126">string</span></span> | <span data-ttu-id="577df-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="577df-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="577df-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="577df-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="577df-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="577df-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="577df-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="577df-130">Required.</span></span> |

<span data-ttu-id="577df-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="577df-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="577df-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="577df-132">The default output type is text/csv.</span></span> <span data-ttu-id="577df-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="577df-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="577df-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="577df-134">Request headers</span></span>

| <span data-ttu-id="577df-135">Nome</span><span class="sxs-lookup"><span data-stu-id="577df-135">Name</span></span>          | <span data-ttu-id="577df-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="577df-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="577df-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="577df-137">Authorization</span></span> | <span data-ttu-id="577df-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="577df-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="577df-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="577df-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="577df-141">CSV</span><span class="sxs-lookup"><span data-stu-id="577df-141">CSV</span></span>

<span data-ttu-id="577df-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="577df-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="577df-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="577df-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="577df-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="577df-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="577df-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="577df-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="577df-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="577df-146">Report Refresh Date</span></span>
- <span data-ttu-id="577df-147">Web</span><span class="sxs-lookup"><span data-stu-id="577df-147">Web</span></span>
- <span data-ttu-id="577df-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="577df-148">Windows Phone</span></span>
- <span data-ttu-id="577df-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="577df-149">Android Phone</span></span>
- <span data-ttu-id="577df-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="577df-150">iPhone</span></span>
- <span data-ttu-id="577df-151">iPad</span><span class="sxs-lookup"><span data-stu-id="577df-151">iPad</span></span>
- <span data-ttu-id="577df-152">Outro</span><span class="sxs-lookup"><span data-stu-id="577df-152">Other</span></span>
- <span data-ttu-id="577df-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="577df-153">Report Date</span></span>
- <span data-ttu-id="577df-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="577df-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="577df-155">JSON</span><span class="sxs-lookup"><span data-stu-id="577df-155">JSON</span></span>

<span data-ttu-id="577df-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="577df-156">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="577df-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="577df-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="577df-158">CSV</span><span class="sxs-lookup"><span data-stu-id="577df-158">CSV</span></span>

<span data-ttu-id="577df-159">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="577df-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="577df-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="577df-160">Request</span></span>

<span data-ttu-id="577df-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="577df-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="577df-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="577df-162">Response</span></span>

<span data-ttu-id="577df-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="577df-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="577df-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="577df-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="577df-165">JSON</span><span class="sxs-lookup"><span data-stu-id="577df-165">JSON</span></span>

<span data-ttu-id="577df-166">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="577df-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="577df-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="577df-167">Request</span></span>

<span data-ttu-id="577df-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="577df-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="577df-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="577df-169">Response</span></span>

<span data-ttu-id="577df-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="577df-170">The following is an example of the response.</span></span>

> <span data-ttu-id="577df-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="577df-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
