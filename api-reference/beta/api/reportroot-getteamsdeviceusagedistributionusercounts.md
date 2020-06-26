---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 60bf9b1d0ee47bb35d6abbb21f3f813442536f70
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896172"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="7b89c-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7b89c-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="7b89c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b89c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b89c-105">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="7b89c-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b89c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b89c-106">Permissions</span></span>

<span data-ttu-id="7b89c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7b89c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7b89c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b89c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b89c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b89c-109">Permission type</span></span>                        | <span data-ttu-id="7b89c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b89c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7b89c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b89c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b89c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b89c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7b89c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b89c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b89c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b89c-114">Not supported.</span></span>                           |
| <span data-ttu-id="7b89c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b89c-115">Application</span></span>                            | <span data-ttu-id="7b89c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b89c-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="7b89c-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7b89c-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7b89c-118">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7b89c-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7b89c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b89c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="7b89c-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7b89c-120">Function parameters</span></span>

<span data-ttu-id="7b89c-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7b89c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7b89c-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7b89c-122">Parameter</span></span> | <span data-ttu-id="7b89c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b89c-123">Type</span></span>   | <span data-ttu-id="7b89c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b89c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7b89c-125">ponto</span><span class="sxs-lookup"><span data-stu-id="7b89c-125">period</span></span>    | <span data-ttu-id="7b89c-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b89c-126">string</span></span> | <span data-ttu-id="7b89c-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7b89c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7b89c-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7b89c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7b89c-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7b89c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7b89c-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b89c-130">Required.</span></span> |

<span data-ttu-id="7b89c-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b89c-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7b89c-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="7b89c-132">The default output type is text/csv.</span></span> <span data-ttu-id="7b89c-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="7b89c-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b89c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b89c-134">Request headers</span></span>

| <span data-ttu-id="7b89c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="7b89c-135">Name</span></span>          | <span data-ttu-id="7b89c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b89c-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7b89c-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b89c-137">Authorization</span></span> | <span data-ttu-id="7b89c-138">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7b89c-138">Bearer {token}.</span></span> <span data-ttu-id="7b89c-139">Required.</span><span class="sxs-lookup"><span data-stu-id="7b89c-139">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7b89c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b89c-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7b89c-141">CSV</span><span class="sxs-lookup"><span data-stu-id="7b89c-141">CSV</span></span>

<span data-ttu-id="7b89c-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7b89c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7b89c-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7b89c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7b89c-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7b89c-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7b89c-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7b89c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7b89c-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7b89c-146">Report Refresh Date</span></span>
- <span data-ttu-id="7b89c-147">Web</span><span class="sxs-lookup"><span data-stu-id="7b89c-147">Web</span></span>
- <span data-ttu-id="7b89c-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7b89c-148">Windows Phone</span></span>
- <span data-ttu-id="7b89c-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="7b89c-149">Android Phone</span></span>
- <span data-ttu-id="7b89c-150">iOS</span><span class="sxs-lookup"><span data-stu-id="7b89c-150">iOS</span></span>
- <span data-ttu-id="7b89c-151">Mac</span><span class="sxs-lookup"><span data-stu-id="7b89c-151">Mac</span></span>
- <span data-ttu-id="7b89c-152">Windows</span><span class="sxs-lookup"><span data-stu-id="7b89c-152">Windows</span></span>
- <span data-ttu-id="7b89c-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7b89c-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7b89c-154">JSON</span><span class="sxs-lookup"><span data-stu-id="7b89c-154">JSON</span></span>

<span data-ttu-id="7b89c-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b89c-155">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b89c-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b89c-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7b89c-157">CSV</span><span class="sxs-lookup"><span data-stu-id="7b89c-157">CSV</span></span>

<span data-ttu-id="7b89c-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="7b89c-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7b89c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b89c-159">Request</span></span>

<span data-ttu-id="7b89c-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b89c-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7b89c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b89c-161">Response</span></span>

<span data-ttu-id="7b89c-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b89c-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7b89c-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7b89c-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7b89c-164">JSON</span><span class="sxs-lookup"><span data-stu-id="7b89c-164">JSON</span></span>

<span data-ttu-id="7b89c-165">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="7b89c-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7b89c-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b89c-166">Request</span></span>

<span data-ttu-id="7b89c-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b89c-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7b89c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b89c-168">Response</span></span>

<span data-ttu-id="7b89c-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b89c-169">The following is an example of the response.</span></span>

> <span data-ttu-id="7b89c-170">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="7b89c-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b89c-171">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7b89c-171">All the properties will be returned from an actual call.</span></span>

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
