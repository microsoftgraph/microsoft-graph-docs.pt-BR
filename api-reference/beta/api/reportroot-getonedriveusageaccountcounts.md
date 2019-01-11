---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.openlocfilehash: 2db065d71e741abe9a3a9fe20e3de62b78115cbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806213"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="40d9d-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="40d9d-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

> <span data-ttu-id="40d9d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="40d9d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40d9d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40d9d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40d9d-107">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="40d9d-107">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="40d9d-108">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="40d9d-108">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="40d9d-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="40d9d-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="40d9d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="40d9d-110">Permissions</span></span>

<span data-ttu-id="40d9d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40d9d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40d9d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40d9d-113">Permission type</span></span>                        | <span data-ttu-id="40d9d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40d9d-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="40d9d-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40d9d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="40d9d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40d9d-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="40d9d-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40d9d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40d9d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40d9d-118">Not supported.</span></span>                           |
| <span data-ttu-id="40d9d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40d9d-119">Application</span></span>                            | <span data-ttu-id="40d9d-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40d9d-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="40d9d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40d9d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="40d9d-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="40d9d-122">Function parameters</span></span>

<span data-ttu-id="40d9d-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="40d9d-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="40d9d-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="40d9d-124">Parameter</span></span> | <span data-ttu-id="40d9d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="40d9d-125">Type</span></span>   | <span data-ttu-id="40d9d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="40d9d-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="40d9d-127">ponto</span><span class="sxs-lookup"><span data-stu-id="40d9d-127">period</span></span>    | <span data-ttu-id="40d9d-128">string</span><span class="sxs-lookup"><span data-stu-id="40d9d-128">string</span></span> | <span data-ttu-id="40d9d-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="40d9d-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="40d9d-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="40d9d-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="40d9d-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="40d9d-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="40d9d-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40d9d-132">Required.</span></span> |

<span data-ttu-id="40d9d-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40d9d-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="40d9d-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="40d9d-134">The default output type is text/csv.</span></span> <span data-ttu-id="40d9d-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="40d9d-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40d9d-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40d9d-136">Request headers</span></span>

| <span data-ttu-id="40d9d-137">Nome</span><span class="sxs-lookup"><span data-stu-id="40d9d-137">Name</span></span>          | <span data-ttu-id="40d9d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="40d9d-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="40d9d-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="40d9d-139">Authorization</span></span> | <span data-ttu-id="40d9d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40d9d-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="40d9d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d9d-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="40d9d-143">CSV</span><span class="sxs-lookup"><span data-stu-id="40d9d-143">CSV</span></span>

<span data-ttu-id="40d9d-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="40d9d-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="40d9d-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="40d9d-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="40d9d-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="40d9d-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="40d9d-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="40d9d-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="40d9d-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="40d9d-148">Report Refresh Date</span></span>
- <span data-ttu-id="40d9d-149">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="40d9d-149">Site Type</span></span>
- <span data-ttu-id="40d9d-150">Total</span><span class="sxs-lookup"><span data-stu-id="40d9d-150">Total</span></span>
- <span data-ttu-id="40d9d-151">Ativo</span><span class="sxs-lookup"><span data-stu-id="40d9d-151">Active</span></span>
- <span data-ttu-id="40d9d-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="40d9d-152">Report Date</span></span>
- <span data-ttu-id="40d9d-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="40d9d-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="40d9d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="40d9d-154">JSON</span></span>

<span data-ttu-id="40d9d-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40d9d-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40d9d-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40d9d-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="40d9d-157">CSV</span><span class="sxs-lookup"><span data-stu-id="40d9d-157">CSV</span></span>

<span data-ttu-id="40d9d-158">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="40d9d-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="40d9d-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40d9d-159">Request</span></span>

<span data-ttu-id="40d9d-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="40d9d-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="40d9d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d9d-161">Response</span></span>

<span data-ttu-id="40d9d-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="40d9d-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="40d9d-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="40d9d-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="40d9d-164">JSON</span><span class="sxs-lookup"><span data-stu-id="40d9d-164">JSON</span></span>

<span data-ttu-id="40d9d-165">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="40d9d-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="40d9d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40d9d-166">Request</span></span>

<span data-ttu-id="40d9d-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="40d9d-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="40d9d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d9d-168">Response</span></span>

<span data-ttu-id="40d9d-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="40d9d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="40d9d-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40d9d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
