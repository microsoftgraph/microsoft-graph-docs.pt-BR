---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
ms.openlocfilehash: b2416b8a4aa257f49807efb3f320fcf16cea4920
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038695"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="0b983-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="0b983-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="0b983-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b983-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b983-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b983-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b983-106">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="0b983-106">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b983-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b983-107">Permissions</span></span>

<span data-ttu-id="0b983-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b983-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b983-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b983-110">Permission type</span></span>                        | <span data-ttu-id="0b983-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b983-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b983-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b983-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b983-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b983-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b983-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b983-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b983-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b983-115">Not supported.</span></span>                           |
| <span data-ttu-id="0b983-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b983-116">Application</span></span>                            | <span data-ttu-id="0b983-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b983-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b983-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b983-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="0b983-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0b983-119">Function parameters</span></span>

<span data-ttu-id="0b983-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0b983-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0b983-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0b983-121">Parameter</span></span> | <span data-ttu-id="0b983-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b983-122">Type</span></span>   | <span data-ttu-id="0b983-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b983-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b983-124">ponto</span><span class="sxs-lookup"><span data-stu-id="0b983-124">period</span></span>    | <span data-ttu-id="0b983-125">string</span><span class="sxs-lookup"><span data-stu-id="0b983-125">string</span></span> | <span data-ttu-id="0b983-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0b983-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b983-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0b983-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b983-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0b983-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0b983-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b983-129">Required.</span></span> |

<span data-ttu-id="0b983-130">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b983-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0b983-131">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="0b983-131">The default output type is text/csv.</span></span> <span data-ttu-id="0b983-132">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="0b983-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b983-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b983-133">Request headers</span></span>

| <span data-ttu-id="0b983-134">Nome</span><span class="sxs-lookup"><span data-stu-id="0b983-134">Name</span></span>          | <span data-ttu-id="0b983-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b983-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0b983-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b983-136">Authorization</span></span> | <span data-ttu-id="0b983-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b983-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0b983-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b983-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0b983-140">CSV</span><span class="sxs-lookup"><span data-stu-id="0b983-140">CSV</span></span>

<span data-ttu-id="0b983-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0b983-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b983-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0b983-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b983-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0b983-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b983-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0b983-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b983-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0b983-145">Report Refresh Date</span></span>
- <span data-ttu-id="0b983-146">Web</span><span class="sxs-lookup"><span data-stu-id="0b983-146">Web</span></span>
- <span data-ttu-id="0b983-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="0b983-147">Windows Phone</span></span>
- <span data-ttu-id="0b983-148">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="0b983-148">Android Phone</span></span>
- <span data-ttu-id="0b983-149">iOS</span><span class="sxs-lookup"><span data-stu-id="0b983-149">iOS</span></span>
- <span data-ttu-id="0b983-150">Mac</span><span class="sxs-lookup"><span data-stu-id="0b983-150">Mac</span></span>
- <span data-ttu-id="0b983-151">Windows</span><span class="sxs-lookup"><span data-stu-id="0b983-151">Windows</span></span>
- <span data-ttu-id="0b983-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0b983-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0b983-153">JSON</span><span class="sxs-lookup"><span data-stu-id="0b983-153">JSON</span></span>

<span data-ttu-id="0b983-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b983-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b983-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b983-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0b983-156">CSV</span><span class="sxs-lookup"><span data-stu-id="0b983-156">CSV</span></span>

<span data-ttu-id="0b983-157">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="0b983-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0b983-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b983-158">Request</span></span>

<span data-ttu-id="0b983-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b983-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0b983-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b983-160">Response</span></span>

<span data-ttu-id="0b983-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b983-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0b983-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0b983-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="0b983-163">JSON</span><span class="sxs-lookup"><span data-stu-id="0b983-163">JSON</span></span>

<span data-ttu-id="0b983-164">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="0b983-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0b983-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b983-165">Request</span></span>

<span data-ttu-id="0b983-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b983-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0b983-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b983-167">Response</span></span>

<span data-ttu-id="0b983-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b983-168">The following is an example of the response.</span></span>

> <span data-ttu-id="0b983-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b983-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
