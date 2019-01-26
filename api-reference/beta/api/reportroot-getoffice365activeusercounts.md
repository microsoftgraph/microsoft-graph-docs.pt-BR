---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9b24008a3ea13308f0d83a2ac6a6ef31ece32469
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575311"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="93210-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="93210-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93210-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="93210-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="93210-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="93210-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="93210-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93210-106">Permissions</span></span>

<span data-ttu-id="93210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93210-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93210-109">Permission type</span></span>                        | <span data-ttu-id="93210-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93210-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="93210-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93210-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93210-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93210-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="93210-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93210-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93210-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93210-114">Not supported.</span></span>                           |
| <span data-ttu-id="93210-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93210-115">Application</span></span>                            | <span data-ttu-id="93210-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93210-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="93210-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93210-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="93210-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="93210-118">Function parameters</span></span>

<span data-ttu-id="93210-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="93210-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="93210-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="93210-120">Parameter</span></span> | <span data-ttu-id="93210-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="93210-121">Type</span></span>   | <span data-ttu-id="93210-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="93210-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="93210-123">ponto</span><span class="sxs-lookup"><span data-stu-id="93210-123">period</span></span>    | <span data-ttu-id="93210-124">string</span><span class="sxs-lookup"><span data-stu-id="93210-124">string</span></span> | <span data-ttu-id="93210-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="93210-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="93210-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="93210-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="93210-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="93210-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="93210-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93210-128">Required.</span></span> |

<span data-ttu-id="93210-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="93210-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="93210-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="93210-130">The default output type is text/csv.</span></span> <span data-ttu-id="93210-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="93210-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93210-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93210-132">Request headers</span></span>

| <span data-ttu-id="93210-133">Nome</span><span class="sxs-lookup"><span data-stu-id="93210-133">Name</span></span>          | <span data-ttu-id="93210-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="93210-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="93210-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="93210-135">Authorization</span></span> | <span data-ttu-id="93210-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93210-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="93210-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="93210-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="93210-139">CSV</span><span class="sxs-lookup"><span data-stu-id="93210-139">CSV</span></span>

<span data-ttu-id="93210-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="93210-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="93210-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="93210-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="93210-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="93210-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="93210-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="93210-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="93210-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="93210-144">Report Refresh Date</span></span>
- <span data-ttu-id="93210-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="93210-145">Office 365</span></span>
- <span data-ttu-id="93210-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="93210-146">Exchange</span></span>
- <span data-ttu-id="93210-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="93210-147">OneDrive</span></span>
- <span data-ttu-id="93210-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="93210-148">SharePoint</span></span>
- <span data-ttu-id="93210-149">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="93210-149">Skype For Business</span></span> 
- <span data-ttu-id="93210-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="93210-150">Yammer</span></span>
- <span data-ttu-id="93210-151">Teams</span><span class="sxs-lookup"><span data-stu-id="93210-151">Teams</span></span>
- <span data-ttu-id="93210-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="93210-152">Report Date</span></span>
- <span data-ttu-id="93210-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="93210-153">Report Period</span></span>

<span data-ttu-id="93210-154">Não há suporte para as seguintes colunas na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="93210-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="93210-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="93210-155">Yammer</span></span>
- <span data-ttu-id="93210-156">Teams</span><span class="sxs-lookup"><span data-stu-id="93210-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="93210-157">JSON</span><span class="sxs-lookup"><span data-stu-id="93210-157">JSON</span></span>

<span data-ttu-id="93210-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93210-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="93210-159">Não há suporte para as seguintes propriedades no objeto **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="93210-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="93210-160">Yammer</span><span class="sxs-lookup"><span data-stu-id="93210-160">yammer</span></span>
- <span data-ttu-id="93210-161">equipes</span><span class="sxs-lookup"><span data-stu-id="93210-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="93210-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93210-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="93210-163">CSV</span><span class="sxs-lookup"><span data-stu-id="93210-163">CSV</span></span>

<span data-ttu-id="93210-164">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="93210-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="93210-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93210-165">Request</span></span>

<span data-ttu-id="93210-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93210-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="93210-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="93210-167">Response</span></span>

<span data-ttu-id="93210-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93210-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="93210-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="93210-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="93210-170">JSON</span><span class="sxs-lookup"><span data-stu-id="93210-170">JSON</span></span>

<span data-ttu-id="93210-171">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="93210-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="93210-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93210-172">Request</span></span>

<span data-ttu-id="93210-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93210-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="93210-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="93210-174">Response</span></span>

<span data-ttu-id="93210-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93210-175">The following is an example of the response.</span></span>

> <span data-ttu-id="93210-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93210-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
