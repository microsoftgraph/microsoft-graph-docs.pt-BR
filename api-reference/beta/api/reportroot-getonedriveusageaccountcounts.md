---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1c588316235f7d6102860da0a8de21a60c5daec0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331802"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="84a9b-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="84a9b-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84a9b-105">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="84a9b-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="84a9b-106">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="84a9b-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="84a9b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="84a9b-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="84a9b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="84a9b-108">Permissions</span></span>

<span data-ttu-id="84a9b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84a9b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84a9b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84a9b-111">Permission type</span></span>                        | <span data-ttu-id="84a9b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84a9b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="84a9b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84a9b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="84a9b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84a9b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="84a9b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84a9b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84a9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a9b-116">Not supported.</span></span>                           |
| <span data-ttu-id="84a9b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84a9b-117">Application</span></span>                            | <span data-ttu-id="84a9b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84a9b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="84a9b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84a9b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="84a9b-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="84a9b-120">Function parameters</span></span>

<span data-ttu-id="84a9b-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="84a9b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="84a9b-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="84a9b-122">Parameter</span></span> | <span data-ttu-id="84a9b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="84a9b-123">Type</span></span>   | <span data-ttu-id="84a9b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a9b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="84a9b-125">ponto</span><span class="sxs-lookup"><span data-stu-id="84a9b-125">period</span></span>    | <span data-ttu-id="84a9b-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a9b-126">string</span></span> | <span data-ttu-id="84a9b-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="84a9b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="84a9b-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="84a9b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="84a9b-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="84a9b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="84a9b-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84a9b-130">Required.</span></span> |

<span data-ttu-id="84a9b-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84a9b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="84a9b-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="84a9b-132">The default output type is text/csv.</span></span> <span data-ttu-id="84a9b-133">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="84a9b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84a9b-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84a9b-134">Request headers</span></span>

| <span data-ttu-id="84a9b-135">Nome</span><span class="sxs-lookup"><span data-stu-id="84a9b-135">Name</span></span>          | <span data-ttu-id="84a9b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a9b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="84a9b-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="84a9b-137">Authorization</span></span> | <span data-ttu-id="84a9b-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84a9b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84a9b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a9b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="84a9b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="84a9b-141">CSV</span></span>

<span data-ttu-id="84a9b-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="84a9b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="84a9b-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="84a9b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="84a9b-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="84a9b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="84a9b-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="84a9b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="84a9b-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="84a9b-146">Report Refresh Date</span></span>
- <span data-ttu-id="84a9b-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="84a9b-147">Site Type</span></span>
- <span data-ttu-id="84a9b-148">Total</span><span class="sxs-lookup"><span data-stu-id="84a9b-148">Total</span></span>
- <span data-ttu-id="84a9b-149">Ativo</span><span class="sxs-lookup"><span data-stu-id="84a9b-149">Active</span></span>
- <span data-ttu-id="84a9b-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="84a9b-150">Report Date</span></span>
- <span data-ttu-id="84a9b-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="84a9b-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="84a9b-152">JSON</span><span class="sxs-lookup"><span data-stu-id="84a9b-152">JSON</span></span>

<span data-ttu-id="84a9b-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84a9b-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84a9b-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84a9b-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="84a9b-155">CSV</span><span class="sxs-lookup"><span data-stu-id="84a9b-155">CSV</span></span>

<span data-ttu-id="84a9b-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="84a9b-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="84a9b-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84a9b-157">Request</span></span>

<span data-ttu-id="84a9b-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84a9b-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="84a9b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a9b-159">Response</span></span>

<span data-ttu-id="84a9b-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84a9b-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="84a9b-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="84a9b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="84a9b-162">JSON</span><span class="sxs-lookup"><span data-stu-id="84a9b-162">JSON</span></span>

<span data-ttu-id="84a9b-163">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="84a9b-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="84a9b-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84a9b-164">Request</span></span>

<span data-ttu-id="84a9b-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84a9b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="84a9b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a9b-166">Response</span></span>

<span data-ttu-id="84a9b-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84a9b-167">The following is an example of the response.</span></span>

> <span data-ttu-id="84a9b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84a9b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
