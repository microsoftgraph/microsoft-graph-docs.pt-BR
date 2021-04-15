---
title: 'reportRoot: getTeamsDeviceUsageTotalUserCounts'
description: Obter o número de usuários exclusivos exclusivos do Microsoft Teams licenciados ou não licenciados por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b65f29260a184193e7689fedff8270d8d5daaf9f
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766897"
---
# <a name="reportroot-getteamsdeviceusagetotalusercounts"></a><span data-ttu-id="9d1d7-103">reportRoot: getTeamsDeviceUsageTotalUserCounts</span><span class="sxs-lookup"><span data-stu-id="9d1d7-103">reportRoot: getTeamsDeviceUsageTotalUserCounts</span></span>

<span data-ttu-id="9d1d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d1d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d1d7-105">Obter o número de usuários exclusivos exclusivos do Microsoft Teams licenciados ou não licenciados por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-105">Get the number of daily unique Microsoft Teams licensed or non-licensed users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d1d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d1d7-106">Permissions</span></span>

<span data-ttu-id="9d1d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d1d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d1d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d1d7-109">Permission type</span></span>                        | <span data-ttu-id="9d1d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d1d7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9d1d7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d1d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d1d7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d1d7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9d1d7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d1d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d1d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-114">Not supported.</span></span>                           |
| <span data-ttu-id="9d1d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d1d7-115">Application</span></span>                            | <span data-ttu-id="9d1d7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d1d7-116">Reports.Read.All</span></span>                         |

><span data-ttu-id="9d1d7-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9d1d7-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="9d1d7-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9d1d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d1d7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageTotalUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="9d1d7-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9d1d7-120">Function parameters</span></span>

<span data-ttu-id="9d1d7-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9d1d7-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9d1d7-122">Parameter</span></span> | <span data-ttu-id="9d1d7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d1d7-123">Type</span></span>   | <span data-ttu-id="9d1d7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d1d7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9d1d7-125">ponto</span><span class="sxs-lookup"><span data-stu-id="9d1d7-125">period</span></span>    | <span data-ttu-id="9d1d7-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d1d7-126">string</span></span> | <span data-ttu-id="9d1d7-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9d1d7-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9d1d7-129">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9d1d7-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-130">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9d1d7-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d1d7-131">Optional query parameters</span></span>

<span data-ttu-id="9d1d7-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9d1d7-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-133">The default output type is text/csv.</span></span> <span data-ttu-id="9d1d7-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData definido como `$format` text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-134">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d1d7-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d1d7-135">Request headers</span></span>

| <span data-ttu-id="9d1d7-136">Nome</span><span class="sxs-lookup"><span data-stu-id="9d1d7-136">Name</span></span>          | <span data-ttu-id="9d1d7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d1d7-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9d1d7-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d1d7-138">Authorization</span></span> | <span data-ttu-id="9d1d7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9d1d7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d1d7-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9d1d7-142">CSV</span><span class="sxs-lookup"><span data-stu-id="9d1d7-142">CSV</span></span>

<span data-ttu-id="9d1d7-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9d1d7-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9d1d7-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9d1d7-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9d1d7-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9d1d7-147">Report Refresh Date</span></span>
- <span data-ttu-id="9d1d7-148">Web</span><span class="sxs-lookup"><span data-stu-id="9d1d7-148">Web</span></span>
- <span data-ttu-id="9d1d7-149">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="9d1d7-149">Windows Phone</span></span>
- <span data-ttu-id="9d1d7-150">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="9d1d7-150">Android Phone</span></span>
- <span data-ttu-id="9d1d7-151">iOS</span><span class="sxs-lookup"><span data-stu-id="9d1d7-151">iOS</span></span>
- <span data-ttu-id="9d1d7-152">Mac</span><span class="sxs-lookup"><span data-stu-id="9d1d7-152">Mac</span></span>
- <span data-ttu-id="9d1d7-153">Windows</span><span class="sxs-lookup"><span data-stu-id="9d1d7-153">Windows</span></span>
- <span data-ttu-id="9d1d7-154">Sistema operacional Chrome</span><span class="sxs-lookup"><span data-stu-id="9d1d7-154">Chrome OS</span></span>
- <span data-ttu-id="9d1d7-155">Linux</span><span class="sxs-lookup"><span data-stu-id="9d1d7-155">Linux</span></span>
- <span data-ttu-id="9d1d7-156">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="9d1d7-156">Report Date</span></span>
- <span data-ttu-id="9d1d7-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9d1d7-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9d1d7-158">JSON</span><span class="sxs-lookup"><span data-stu-id="9d1d7-158">JSON</span></span>

<span data-ttu-id="9d1d7-159">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-159">If successful, this method returns a `200 OK` response code and a [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d1d7-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d1d7-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9d1d7-161">CSV</span><span class="sxs-lookup"><span data-stu-id="9d1d7-161">CSV</span></span>

<span data-ttu-id="9d1d7-162">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9d1d7-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d1d7-163">Request</span></span>

<span data-ttu-id="9d1d7-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagetotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageTotalUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="9d1d7-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d1d7-165">Response</span></span>

<span data-ttu-id="9d1d7-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9d1d7-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Chrome OS,Linux,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="9d1d7-168">JSON</span><span class="sxs-lookup"><span data-stu-id="9d1d7-168">JSON</span></span>

<span data-ttu-id="9d1d7-169">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9d1d7-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d1d7-170">Request</span></span>

<span data-ttu-id="9d1d7-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagetotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageTotalUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="9d1d7-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d1d7-172">Response</span></span>

<span data-ttu-id="9d1d7-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-173">The following is an example of the response.</span></span>

> <span data-ttu-id="9d1d7-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9d1d7-174">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
      "chromeOS": 10, 
      "linux": 5, 
      "reportDate": "2017-09-01", 
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
