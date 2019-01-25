---
title: 'reportRoot: getOneDriveUsageStorage'
description: Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4274740947e9160817cf874f9d2105b24d71de86
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510012"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="60448-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="60448-103">reportRoot: getOneDriveUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60448-104">Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="60448-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="60448-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="60448-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="60448-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60448-106">Permissions</span></span>

<span data-ttu-id="60448-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60448-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60448-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60448-109">Permission type</span></span>                        | <span data-ttu-id="60448-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60448-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="60448-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60448-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60448-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60448-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="60448-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60448-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60448-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60448-114">Not supported.</span></span>                           |
| <span data-ttu-id="60448-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60448-115">Application</span></span>                            | <span data-ttu-id="60448-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60448-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="60448-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60448-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="60448-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="60448-118">Function parameters</span></span>

<span data-ttu-id="60448-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="60448-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="60448-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="60448-120">Parameter</span></span> | <span data-ttu-id="60448-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="60448-121">Type</span></span>   | <span data-ttu-id="60448-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="60448-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="60448-123">ponto</span><span class="sxs-lookup"><span data-stu-id="60448-123">period</span></span>    | <span data-ttu-id="60448-124">string</span><span class="sxs-lookup"><span data-stu-id="60448-124">string</span></span> | <span data-ttu-id="60448-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="60448-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="60448-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="60448-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="60448-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="60448-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="60448-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60448-128">Required.</span></span> |

<span data-ttu-id="60448-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60448-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="60448-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="60448-130">The default output type is text/csv.</span></span> <span data-ttu-id="60448-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="60448-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60448-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60448-132">Request headers</span></span>

| <span data-ttu-id="60448-133">Nome</span><span class="sxs-lookup"><span data-stu-id="60448-133">Name</span></span>          | <span data-ttu-id="60448-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="60448-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="60448-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="60448-135">Authorization</span></span> | <span data-ttu-id="60448-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60448-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="60448-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="60448-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="60448-139">CSV</span><span class="sxs-lookup"><span data-stu-id="60448-139">CSV</span></span>

<span data-ttu-id="60448-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="60448-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="60448-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="60448-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="60448-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="60448-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="60448-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="60448-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="60448-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="60448-144">Report Refresh Date</span></span>
- <span data-ttu-id="60448-145">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="60448-145">Site Type</span></span>
- <span data-ttu-id="60448-146">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="60448-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="60448-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="60448-147">Report Date</span></span>
- <span data-ttu-id="60448-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="60448-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="60448-149">JSON</span><span class="sxs-lookup"><span data-stu-id="60448-149">JSON</span></span>

<span data-ttu-id="60448-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[siteUsageStorage](../resources/siteusagestorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60448-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60448-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60448-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="60448-152">CSV</span><span class="sxs-lookup"><span data-stu-id="60448-152">CSV</span></span>

<span data-ttu-id="60448-153">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="60448-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="60448-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60448-154">Request</span></span>

<span data-ttu-id="60448-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60448-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="60448-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="60448-156">Response</span></span>

<span data-ttu-id="60448-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60448-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="60448-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="60448-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="60448-159">JSON</span><span class="sxs-lookup"><span data-stu-id="60448-159">JSON</span></span>

<span data-ttu-id="60448-160">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="60448-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="60448-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60448-161">Request</span></span>

<span data-ttu-id="60448-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60448-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="60448-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="60448-163">Response</span></span>

<span data-ttu-id="60448-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60448-164">The following is an example of the response.</span></span>

> <span data-ttu-id="60448-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60448-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "storageUsedInBytes": 132654293197, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusagestorage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
