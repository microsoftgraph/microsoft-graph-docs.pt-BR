---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0c1fa1bf6f42b7fb24d1a4a7db7c50ad4431e8b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576350"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="ce0c9-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="ce0c9-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce0c9-104">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="ce0c9-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="ce0c9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce0c9-106">Permissions</span></span>

<span data-ttu-id="ce0c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce0c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce0c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce0c9-109">Permission type</span></span>                        | <span data-ttu-id="ce0c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce0c9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ce0c9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce0c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce0c9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce0c9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ce0c9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce0c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-114">Not supported.</span></span>                           |
| <span data-ttu-id="ce0c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce0c9-115">Application</span></span>                            | <span data-ttu-id="ce0c9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce0c9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ce0c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce0c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ce0c9-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ce0c9-118">Function parameters</span></span>

<span data-ttu-id="ce0c9-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ce0c9-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ce0c9-120">Parameter</span></span> | <span data-ttu-id="ce0c9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce0c9-121">Type</span></span>   | <span data-ttu-id="ce0c9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce0c9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ce0c9-123">ponto</span><span class="sxs-lookup"><span data-stu-id="ce0c9-123">period</span></span>    | <span data-ttu-id="ce0c9-124">string</span><span class="sxs-lookup"><span data-stu-id="ce0c9-124">string</span></span> | <span data-ttu-id="ce0c9-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ce0c9-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ce0c9-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ce0c9-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-128">Required.</span></span> |

<span data-ttu-id="ce0c9-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ce0c9-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-130">The default output type is text/csv.</span></span> <span data-ttu-id="ce0c9-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce0c9-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c9-132">Request headers</span></span>

| <span data-ttu-id="ce0c9-133">Nome</span><span class="sxs-lookup"><span data-stu-id="ce0c9-133">Name</span></span>          | <span data-ttu-id="ce0c9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce0c9-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ce0c9-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce0c9-135">Authorization</span></span> | <span data-ttu-id="ce0c9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ce0c9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c9-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ce0c9-139">CSV</span><span class="sxs-lookup"><span data-stu-id="ce0c9-139">CSV</span></span>

<span data-ttu-id="ce0c9-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ce0c9-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ce0c9-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ce0c9-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ce0c9-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ce0c9-144">Report Refresh Date</span></span>
- <span data-ttu-id="ce0c9-145">Total</span><span class="sxs-lookup"><span data-stu-id="ce0c9-145">Total</span></span>
- <span data-ttu-id="ce0c9-146">Ativo</span><span class="sxs-lookup"><span data-stu-id="ce0c9-146">Active</span></span>
- <span data-ttu-id="ce0c9-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ce0c9-147">Report Date</span></span>
- <span data-ttu-id="ce0c9-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ce0c9-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ce0c9-149">JSON</span><span class="sxs-lookup"><span data-stu-id="ce0c9-149">JSON</span></span>

<span data-ttu-id="ce0c9-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce0c9-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce0c9-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ce0c9-152">CSV</span><span class="sxs-lookup"><span data-stu-id="ce0c9-152">CSV</span></span>

<span data-ttu-id="ce0c9-153">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ce0c9-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c9-154">Request</span></span>

<span data-ttu-id="ce0c9-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ce0c9-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c9-156">Response</span></span>

<span data-ttu-id="ce0c9-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ce0c9-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="ce0c9-159">JSON</span><span class="sxs-lookup"><span data-stu-id="ce0c9-159">JSON</span></span>

<span data-ttu-id="ce0c9-160">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ce0c9-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c9-161">Request</span></span>

<span data-ttu-id="ce0c9-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ce0c9-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c9-163">Response</span></span>

<span data-ttu-id="ce0c9-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-164">The following is an example of the response.</span></span>

> <span data-ttu-id="ce0c9-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce0c9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 26, 
      "active": 5, 
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
