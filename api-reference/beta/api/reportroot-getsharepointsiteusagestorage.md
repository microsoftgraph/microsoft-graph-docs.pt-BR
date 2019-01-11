---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório.
localization_priority: Normal
ms.openlocfilehash: 231da76d9009966fd14e98badf52aa84a231d7b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807333"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="e4015-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="e4015-103">reportRoot: getSharePointSiteUsageStorage</span></span>

> <span data-ttu-id="e4015-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4015-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4015-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4015-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4015-106">Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="e4015-106">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="e4015-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="e4015-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4015-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4015-108">Permissions</span></span>

<span data-ttu-id="e4015-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4015-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4015-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4015-111">Permission type</span></span>                        | <span data-ttu-id="e4015-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4015-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e4015-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4015-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4015-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4015-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e4015-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4015-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4015-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4015-116">Not supported.</span></span>                           |
| <span data-ttu-id="e4015-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4015-117">Application</span></span>                            | <span data-ttu-id="e4015-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4015-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e4015-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4015-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e4015-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e4015-120">Function parameters</span></span>

<span data-ttu-id="e4015-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e4015-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e4015-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e4015-122">Parameter</span></span> | <span data-ttu-id="e4015-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4015-123">Type</span></span>   | <span data-ttu-id="e4015-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4015-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e4015-125">ponto</span><span class="sxs-lookup"><span data-stu-id="e4015-125">period</span></span>    | <span data-ttu-id="e4015-126">string</span><span class="sxs-lookup"><span data-stu-id="e4015-126">string</span></span> | <span data-ttu-id="e4015-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e4015-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e4015-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e4015-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e4015-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e4015-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e4015-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4015-130">Required.</span></span> |

<span data-ttu-id="e4015-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4015-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e4015-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="e4015-132">The default output type is text/csv.</span></span> <span data-ttu-id="e4015-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="e4015-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4015-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4015-134">Request headers</span></span>

| <span data-ttu-id="e4015-135">Nome</span><span class="sxs-lookup"><span data-stu-id="e4015-135">Name</span></span>          | <span data-ttu-id="e4015-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4015-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e4015-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4015-137">Authorization</span></span> | <span data-ttu-id="e4015-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4015-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e4015-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4015-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e4015-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e4015-141">CSV</span></span>

<span data-ttu-id="e4015-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e4015-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e4015-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4015-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e4015-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e4015-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e4015-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e4015-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e4015-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e4015-146">Report Refresh Date</span></span>
- <span data-ttu-id="e4015-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="e4015-147">Site Type</span></span>
- <span data-ttu-id="e4015-148">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="e4015-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="e4015-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e4015-149">Report Date</span></span>
- <span data-ttu-id="e4015-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e4015-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e4015-151">JSON</span><span class="sxs-lookup"><span data-stu-id="e4015-151">JSON</span></span>

<span data-ttu-id="e4015-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[siteUsageStorage](../resources/siteusagestorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4015-152">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4015-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4015-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e4015-154">CSV</span><span class="sxs-lookup"><span data-stu-id="e4015-154">CSV</span></span>

<span data-ttu-id="e4015-155">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="e4015-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e4015-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4015-156">Request</span></span>

<span data-ttu-id="e4015-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4015-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e4015-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4015-158">Response</span></span>

<span data-ttu-id="e4015-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4015-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e4015-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e4015-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e4015-161">JSON</span><span class="sxs-lookup"><span data-stu-id="e4015-161">JSON</span></span>

<span data-ttu-id="e4015-162">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="e4015-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e4015-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4015-163">Request</span></span>

<span data-ttu-id="e4015-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4015-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e4015-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4015-165">Response</span></span>

<span data-ttu-id="e4015-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4015-166">The following is an example of the response.</span></span>

> <span data-ttu-id="e4015-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4015-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 171835798971, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
