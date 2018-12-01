---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.
ms.openlocfilehash: d3166c6e8e0e2edf0eb766d87171cd53886416b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041135"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="af696-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="af696-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

> <span data-ttu-id="af696-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af696-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af696-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af696-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af696-106">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="af696-106">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="af696-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="af696-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="af696-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="af696-108">Permissions</span></span>

<span data-ttu-id="af696-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="af696-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af696-111">Permission type</span></span>                        | <span data-ttu-id="af696-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af696-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="af696-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af696-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="af696-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="af696-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="af696-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af696-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af696-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af696-116">Not supported.</span></span>                           |
| <span data-ttu-id="af696-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af696-117">Application</span></span>                            | <span data-ttu-id="af696-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="af696-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="af696-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af696-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="af696-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="af696-120">Function parameters</span></span>

<span data-ttu-id="af696-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="af696-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="af696-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="af696-122">Parameter</span></span> | <span data-ttu-id="af696-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="af696-123">Type</span></span>   | <span data-ttu-id="af696-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="af696-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="af696-125">ponto</span><span class="sxs-lookup"><span data-stu-id="af696-125">period</span></span>    | <span data-ttu-id="af696-126">string</span><span class="sxs-lookup"><span data-stu-id="af696-126">string</span></span> | <span data-ttu-id="af696-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="af696-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="af696-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="af696-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="af696-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="af696-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="af696-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af696-130">Required.</span></span> |

<span data-ttu-id="af696-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af696-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="af696-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="af696-132">The default output type is text/csv.</span></span> <span data-ttu-id="af696-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="af696-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af696-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af696-134">Request headers</span></span>

| <span data-ttu-id="af696-135">Nome</span><span class="sxs-lookup"><span data-stu-id="af696-135">Name</span></span>          | <span data-ttu-id="af696-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="af696-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="af696-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="af696-137">Authorization</span></span> | <span data-ttu-id="af696-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af696-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="af696-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="af696-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="af696-141">CSV</span><span class="sxs-lookup"><span data-stu-id="af696-141">CSV</span></span>

<span data-ttu-id="af696-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="af696-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="af696-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="af696-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="af696-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="af696-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="af696-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="af696-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="af696-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="af696-146">Report Refresh Date</span></span>
- <span data-ttu-id="af696-147">Total</span><span class="sxs-lookup"><span data-stu-id="af696-147">Total</span></span>
- <span data-ttu-id="af696-148">Ativo</span><span class="sxs-lookup"><span data-stu-id="af696-148">Active</span></span>
- <span data-ttu-id="af696-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="af696-149">Report Date</span></span>
- <span data-ttu-id="af696-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="af696-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="af696-151">JSON</span><span class="sxs-lookup"><span data-stu-id="af696-151">JSON</span></span>

<span data-ttu-id="af696-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af696-152">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af696-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af696-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="af696-154">CSV</span><span class="sxs-lookup"><span data-stu-id="af696-154">CSV</span></span>

<span data-ttu-id="af696-155">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="af696-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="af696-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af696-156">Request</span></span>

<span data-ttu-id="af696-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af696-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="af696-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="af696-158">Response</span></span>

<span data-ttu-id="af696-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="af696-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="af696-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="af696-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="af696-161">JSON</span><span class="sxs-lookup"><span data-stu-id="af696-161">JSON</span></span>

<span data-ttu-id="af696-162">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="af696-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="af696-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af696-163">Request</span></span>

<span data-ttu-id="af696-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af696-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="af696-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="af696-165">Response</span></span>

<span data-ttu-id="af696-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="af696-166">The following is an example of the response.</span></span>

> <span data-ttu-id="af696-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af696-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 50, 
      "active": 41, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
