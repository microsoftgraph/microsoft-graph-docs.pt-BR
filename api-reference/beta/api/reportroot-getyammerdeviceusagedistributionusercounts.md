---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 64e79ab2a1c88b63f6902cac266765fe7256c3c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052970"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="e3115-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="e3115-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="e3115-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3115-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3115-105">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e3115-105">Get the number of users by device type.</span></span>

> <span data-ttu-id="e3115-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="e3115-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3115-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3115-107">Permissions</span></span>

<span data-ttu-id="e3115-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3115-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3115-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3115-110">Permission type</span></span>                        | <span data-ttu-id="e3115-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3115-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e3115-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3115-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3115-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3115-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e3115-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3115-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3115-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3115-115">Not supported.</span></span>                           |
| <span data-ttu-id="e3115-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3115-116">Application</span></span>                            | <span data-ttu-id="e3115-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3115-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="e3115-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e3115-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e3115-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e3115-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e3115-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3115-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e3115-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e3115-121">Function parameters</span></span>

<span data-ttu-id="e3115-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e3115-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e3115-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e3115-123">Parameter</span></span> | <span data-ttu-id="e3115-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3115-124">Type</span></span>   | <span data-ttu-id="e3115-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3115-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e3115-126">ponto</span><span class="sxs-lookup"><span data-stu-id="e3115-126">period</span></span>    | <span data-ttu-id="e3115-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3115-127">string</span></span> | <span data-ttu-id="e3115-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e3115-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e3115-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e3115-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e3115-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e3115-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e3115-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3115-131">Required.</span></span> |

<span data-ttu-id="e3115-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3115-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e3115-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="e3115-133">The default output type is text/csv.</span></span> <span data-ttu-id="e3115-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e3115-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3115-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3115-135">Request headers</span></span>

| <span data-ttu-id="e3115-136">Nome</span><span class="sxs-lookup"><span data-stu-id="e3115-136">Name</span></span>          | <span data-ttu-id="e3115-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3115-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e3115-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3115-138">Authorization</span></span> | <span data-ttu-id="e3115-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3115-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e3115-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3115-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e3115-142">CSV</span><span class="sxs-lookup"><span data-stu-id="e3115-142">CSV</span></span>

<span data-ttu-id="e3115-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e3115-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e3115-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e3115-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e3115-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e3115-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e3115-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e3115-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e3115-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e3115-147">Report Refresh Date</span></span>
- <span data-ttu-id="e3115-148">Web</span><span class="sxs-lookup"><span data-stu-id="e3115-148">Web</span></span>
- <span data-ttu-id="e3115-149">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e3115-149">Windows Phone</span></span>
- <span data-ttu-id="e3115-150">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="e3115-150">Android Phone</span></span>
- <span data-ttu-id="e3115-151">iPhone</span><span class="sxs-lookup"><span data-stu-id="e3115-151">iPhone</span></span>
- <span data-ttu-id="e3115-152">iPad</span><span class="sxs-lookup"><span data-stu-id="e3115-152">iPad</span></span>
- <span data-ttu-id="e3115-153">Outro</span><span class="sxs-lookup"><span data-stu-id="e3115-153">Other</span></span>
- <span data-ttu-id="e3115-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e3115-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e3115-155">JSON</span><span class="sxs-lookup"><span data-stu-id="e3115-155">JSON</span></span>

<span data-ttu-id="e3115-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3115-156">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3115-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3115-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e3115-158">CSV</span><span class="sxs-lookup"><span data-stu-id="e3115-158">CSV</span></span>

<span data-ttu-id="e3115-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="e3115-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e3115-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3115-160">Request</span></span>

<span data-ttu-id="e3115-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3115-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="e3115-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3115-162">Response</span></span>

<span data-ttu-id="e3115-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3115-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e3115-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e3115-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```

### <a name="json"></a><span data-ttu-id="e3115-165">JSON</span><span class="sxs-lookup"><span data-stu-id="e3115-165">JSON</span></span>

<span data-ttu-id="e3115-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e3115-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e3115-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3115-167">Request</span></span>

<span data-ttu-id="e3115-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3115-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="e3115-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3115-169">Response</span></span>

<span data-ttu-id="e3115-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3115-170">The following is an example of the response.</span></span>

> <span data-ttu-id="e3115-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3115-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 138, 
      "windowsPhone": 1, 
      "androidPhone": 29, 
      "iPhone": 40, 
      "iPad": 2, 
      "other": 2, 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


