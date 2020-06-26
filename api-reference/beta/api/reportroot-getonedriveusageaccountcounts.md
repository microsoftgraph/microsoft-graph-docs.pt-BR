---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2dec3f6ea849c3536f7bd976b963cf082a2ce5ff
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896753"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="128ec-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="128ec-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="128ec-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="128ec-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="128ec-106">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="128ec-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="128ec-107">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="128ec-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="128ec-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do onedrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="128ec-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="128ec-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="128ec-109">Permissions</span></span>

<span data-ttu-id="128ec-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="128ec-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="128ec-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="128ec-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="128ec-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="128ec-112">Permission type</span></span>                        | <span data-ttu-id="128ec-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="128ec-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="128ec-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="128ec-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="128ec-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="128ec-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="128ec-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="128ec-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="128ec-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="128ec-117">Not supported.</span></span>                           |
| <span data-ttu-id="128ec-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="128ec-118">Application</span></span>                            | <span data-ttu-id="128ec-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="128ec-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="128ec-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="128ec-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="128ec-121">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="128ec-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="128ec-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="128ec-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="128ec-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="128ec-123">Function parameters</span></span>

<span data-ttu-id="128ec-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="128ec-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="128ec-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="128ec-125">Parameter</span></span> | <span data-ttu-id="128ec-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="128ec-126">Type</span></span>   | <span data-ttu-id="128ec-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="128ec-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="128ec-128">ponto</span><span class="sxs-lookup"><span data-stu-id="128ec-128">period</span></span>    | <span data-ttu-id="128ec-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="128ec-129">string</span></span> | <span data-ttu-id="128ec-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="128ec-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="128ec-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="128ec-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="128ec-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="128ec-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="128ec-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="128ec-133">Required.</span></span> |

<span data-ttu-id="128ec-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="128ec-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="128ec-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="128ec-135">The default output type is text/csv.</span></span> <span data-ttu-id="128ec-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="128ec-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="128ec-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="128ec-137">Request headers</span></span>

| <span data-ttu-id="128ec-138">Nome</span><span class="sxs-lookup"><span data-stu-id="128ec-138">Name</span></span>          | <span data-ttu-id="128ec-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="128ec-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="128ec-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="128ec-140">Authorization</span></span> | <span data-ttu-id="128ec-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="128ec-141">Bearer {token}.</span></span> <span data-ttu-id="128ec-142">Required.</span><span class="sxs-lookup"><span data-stu-id="128ec-142">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="128ec-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="128ec-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="128ec-144">CSV</span><span class="sxs-lookup"><span data-stu-id="128ec-144">CSV</span></span>

<span data-ttu-id="128ec-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="128ec-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="128ec-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="128ec-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="128ec-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="128ec-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="128ec-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="128ec-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="128ec-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="128ec-149">Report Refresh Date</span></span>
- <span data-ttu-id="128ec-150">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="128ec-150">Site Type</span></span>
- <span data-ttu-id="128ec-151">Total</span><span class="sxs-lookup"><span data-stu-id="128ec-151">Total</span></span>
- <span data-ttu-id="128ec-152">Ativo</span><span class="sxs-lookup"><span data-stu-id="128ec-152">Active</span></span>
- <span data-ttu-id="128ec-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="128ec-153">Report Date</span></span>
- <span data-ttu-id="128ec-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="128ec-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="128ec-155">JSON</span><span class="sxs-lookup"><span data-stu-id="128ec-155">JSON</span></span>

<span data-ttu-id="128ec-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="128ec-156">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="128ec-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="128ec-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="128ec-158">CSV</span><span class="sxs-lookup"><span data-stu-id="128ec-158">CSV</span></span>

<span data-ttu-id="128ec-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="128ec-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="128ec-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="128ec-160">Request</span></span>

<span data-ttu-id="128ec-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="128ec-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="128ec-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="128ec-162">Response</span></span>

<span data-ttu-id="128ec-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="128ec-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="128ec-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="128ec-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="128ec-165">JSON</span><span class="sxs-lookup"><span data-stu-id="128ec-165">JSON</span></span>

<span data-ttu-id="128ec-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="128ec-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="128ec-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="128ec-167">Request</span></span>

<span data-ttu-id="128ec-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="128ec-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="128ec-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="128ec-169">Response</span></span>

<span data-ttu-id="128ec-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="128ec-170">The following is an example of the response.</span></span>

> <span data-ttu-id="128ec-171">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="128ec-171">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="128ec-172">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="128ec-172">All the properties will be returned from an actual call.</span></span>

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
