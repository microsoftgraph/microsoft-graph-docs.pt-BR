---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9b06042772ee1889e568780098013c0b78ff6e47
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571678"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="5ce91-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="5ce91-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ce91-104">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5ce91-104">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="5ce91-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="5ce91-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ce91-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ce91-106">Permissions</span></span>

<span data-ttu-id="5ce91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ce91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ce91-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ce91-109">Permission type</span></span>                        | <span data-ttu-id="5ce91-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ce91-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5ce91-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ce91-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ce91-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ce91-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5ce91-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ce91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ce91-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ce91-114">Not supported.</span></span>                           |
| <span data-ttu-id="5ce91-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ce91-115">Application</span></span>                            | <span data-ttu-id="5ce91-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ce91-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5ce91-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ce91-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5ce91-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5ce91-118">Function parameters</span></span>

<span data-ttu-id="5ce91-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5ce91-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5ce91-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5ce91-120">Parameter</span></span> | <span data-ttu-id="5ce91-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ce91-121">Type</span></span>   | <span data-ttu-id="5ce91-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ce91-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5ce91-123">ponto</span><span class="sxs-lookup"><span data-stu-id="5ce91-123">period</span></span>    | <span data-ttu-id="5ce91-124">string</span><span class="sxs-lookup"><span data-stu-id="5ce91-124">string</span></span> | <span data-ttu-id="5ce91-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5ce91-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5ce91-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5ce91-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5ce91-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5ce91-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5ce91-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ce91-128">Required.</span></span> |

<span data-ttu-id="5ce91-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce91-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5ce91-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="5ce91-130">The default output type is text/csv.</span></span> <span data-ttu-id="5ce91-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="5ce91-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ce91-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce91-132">Request headers</span></span>

| <span data-ttu-id="5ce91-133">Nome</span><span class="sxs-lookup"><span data-stu-id="5ce91-133">Name</span></span>          | <span data-ttu-id="5ce91-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ce91-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5ce91-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ce91-135">Authorization</span></span> | <span data-ttu-id="5ce91-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ce91-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5ce91-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce91-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5ce91-139">CSV</span><span class="sxs-lookup"><span data-stu-id="5ce91-139">CSV</span></span>

<span data-ttu-id="5ce91-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5ce91-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5ce91-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce91-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5ce91-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5ce91-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5ce91-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5ce91-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5ce91-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5ce91-144">Report Refresh Date</span></span>
- <span data-ttu-id="5ce91-145">Total</span><span class="sxs-lookup"><span data-stu-id="5ce91-145">Total</span></span>
- <span data-ttu-id="5ce91-146">Ativo</span><span class="sxs-lookup"><span data-stu-id="5ce91-146">Active</span></span>
- <span data-ttu-id="5ce91-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5ce91-147">Report Date</span></span>
- <span data-ttu-id="5ce91-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5ce91-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5ce91-149">JSON</span><span class="sxs-lookup"><span data-stu-id="5ce91-149">JSON</span></span>

<span data-ttu-id="5ce91-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce91-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ce91-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ce91-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5ce91-152">CSV</span><span class="sxs-lookup"><span data-stu-id="5ce91-152">CSV</span></span>

<span data-ttu-id="5ce91-153">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="5ce91-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5ce91-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce91-154">Request</span></span>

<span data-ttu-id="5ce91-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ce91-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5ce91-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce91-156">Response</span></span>

<span data-ttu-id="5ce91-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce91-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5ce91-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5ce91-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5ce91-159">JSON</span><span class="sxs-lookup"><span data-stu-id="5ce91-159">JSON</span></span>

<span data-ttu-id="5ce91-160">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="5ce91-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5ce91-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce91-161">Request</span></span>

<span data-ttu-id="5ce91-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ce91-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5ce91-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce91-163">Response</span></span>

<span data-ttu-id="5ce91-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce91-164">The following is an example of the response.</span></span>

> <span data-ttu-id="5ce91-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ce91-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 5344, 
      "active": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitygroupcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
