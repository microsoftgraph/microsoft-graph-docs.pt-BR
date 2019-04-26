---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7f468e46d64dae5bb4a940b2d08f7374a56c3d3a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331409"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="6bcb0-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6bcb0-103">reportRoot: getYammerGroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bcb0-104">Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="6bcb0-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="6bcb0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bcb0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bcb0-106">Permissions</span></span>

<span data-ttu-id="6bcb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bcb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bcb0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bcb0-109">Permission type</span></span>                        | <span data-ttu-id="6bcb0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bcb0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6bcb0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bcb0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bcb0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bcb0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6bcb0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bcb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bcb0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-114">Not supported.</span></span>                           |
| <span data-ttu-id="6bcb0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bcb0-115">Application</span></span>                            | <span data-ttu-id="6bcb0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bcb0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6bcb0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bcb0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6bcb0-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6bcb0-118">Function parameters</span></span>

<span data-ttu-id="6bcb0-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6bcb0-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6bcb0-120">Parameter</span></span> | <span data-ttu-id="6bcb0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bcb0-121">Type</span></span>   | <span data-ttu-id="6bcb0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bcb0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6bcb0-123">ponto</span><span class="sxs-lookup"><span data-stu-id="6bcb0-123">period</span></span>    | <span data-ttu-id="6bcb0-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bcb0-124">string</span></span> | <span data-ttu-id="6bcb0-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6bcb0-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6bcb0-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6bcb0-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-128">Required.</span></span> |

<span data-ttu-id="6bcb0-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6bcb0-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-130">The default output type is text/csv.</span></span> <span data-ttu-id="6bcb0-131">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bcb0-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bcb0-132">Request headers</span></span>

| <span data-ttu-id="6bcb0-133">Nome</span><span class="sxs-lookup"><span data-stu-id="6bcb0-133">Name</span></span>          | <span data-ttu-id="6bcb0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bcb0-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6bcb0-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bcb0-135">Authorization</span></span> | <span data-ttu-id="6bcb0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6bcb0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bcb0-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6bcb0-139">CSV</span><span class="sxs-lookup"><span data-stu-id="6bcb0-139">CSV</span></span>

<span data-ttu-id="6bcb0-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6bcb0-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6bcb0-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6bcb0-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6bcb0-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6bcb0-144">Report Refresh Date</span></span>
- <span data-ttu-id="6bcb0-145">Curtidos</span><span class="sxs-lookup"><span data-stu-id="6bcb0-145">Liked</span></span>
- <span data-ttu-id="6bcb0-146">Postados</span><span class="sxs-lookup"><span data-stu-id="6bcb0-146">Posted</span></span>
- <span data-ttu-id="6bcb0-147">Ler</span><span class="sxs-lookup"><span data-stu-id="6bcb0-147">Read</span></span>
- <span data-ttu-id="6bcb0-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="6bcb0-148">Report Date</span></span>
- <span data-ttu-id="6bcb0-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6bcb0-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6bcb0-150">JSON</span><span class="sxs-lookup"><span data-stu-id="6bcb0-150">JSON</span></span>

<span data-ttu-id="6bcb0-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-151">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bcb0-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bcb0-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6bcb0-153">CSV</span><span class="sxs-lookup"><span data-stu-id="6bcb0-153">CSV</span></span>

<span data-ttu-id="6bcb0-154">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6bcb0-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bcb0-155">Request</span></span>

<span data-ttu-id="6bcb0-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6bcb0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bcb0-157">Response</span></span>

<span data-ttu-id="6bcb0-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6bcb0-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="6bcb0-160">JSON</span><span class="sxs-lookup"><span data-stu-id="6bcb0-160">JSON</span></span>

<span data-ttu-id="6bcb0-161">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6bcb0-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bcb0-162">Request</span></span>

<span data-ttu-id="6bcb0-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6bcb0-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bcb0-164">Response</span></span>

<span data-ttu-id="6bcb0-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-165">The following is an example of the response.</span></span>

> <span data-ttu-id="6bcb0-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bcb0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 13, 
      "posted": 50, 
      "read": 69, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
