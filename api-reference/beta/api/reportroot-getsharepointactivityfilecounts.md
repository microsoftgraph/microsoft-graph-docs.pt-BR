---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 406cdc4db1a068fe5f877abd73ec9afa10a911eb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331721"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="d4e08-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d4e08-103">reportRoot: getSharePointActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e08-104">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d4e08-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="d4e08-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="d4e08-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4e08-106">Permissions</span></span>

<span data-ttu-id="d4e08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4e08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e08-109">Permission type</span></span>                        | <span data-ttu-id="d4e08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4e08-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d4e08-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4e08-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4e08-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d4e08-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4e08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e08-114">Not supported.</span></span>                           |
| <span data-ttu-id="d4e08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4e08-115">Application</span></span>                            | <span data-ttu-id="d4e08-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4e08-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d4e08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e08-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d4e08-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d4e08-118">Function parameters</span></span>

<span data-ttu-id="d4e08-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d4e08-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d4e08-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4e08-120">Parameter</span></span> | <span data-ttu-id="d4e08-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4e08-121">Type</span></span>   | <span data-ttu-id="d4e08-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e08-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d4e08-123">ponto</span><span class="sxs-lookup"><span data-stu-id="d4e08-123">period</span></span>    | <span data-ttu-id="d4e08-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4e08-124">string</span></span> | <span data-ttu-id="d4e08-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d4e08-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d4e08-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d4e08-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d4e08-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d4e08-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d4e08-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e08-128">Required.</span></span> |

<span data-ttu-id="d4e08-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e08-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d4e08-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d4e08-130">The default output type is text/csv.</span></span> <span data-ttu-id="d4e08-131">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e08-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4e08-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e08-132">Request headers</span></span>

| <span data-ttu-id="d4e08-133">Nome</span><span class="sxs-lookup"><span data-stu-id="d4e08-133">Name</span></span>          | <span data-ttu-id="d4e08-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e08-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d4e08-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e08-135">Authorization</span></span> | <span data-ttu-id="d4e08-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e08-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d4e08-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e08-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d4e08-139">CSV</span><span class="sxs-lookup"><span data-stu-id="d4e08-139">CSV</span></span>

<span data-ttu-id="d4e08-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d4e08-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d4e08-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e08-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d4e08-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d4e08-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d4e08-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d4e08-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d4e08-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d4e08-144">Report Refresh Date</span></span>
- <span data-ttu-id="d4e08-145">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="d4e08-145">Viewed Or Edited</span></span>
- <span data-ttu-id="d4e08-146">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="d4e08-146">Synced</span></span>
- <span data-ttu-id="d4e08-147">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="d4e08-147">Shared Internally</span></span>
- <span data-ttu-id="d4e08-148">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="d4e08-148">Shared Externally</span></span>
- <span data-ttu-id="d4e08-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d4e08-149">Report Date</span></span>
- <span data-ttu-id="d4e08-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d4e08-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d4e08-151">JSON</span><span class="sxs-lookup"><span data-stu-id="d4e08-151">JSON</span></span>

<span data-ttu-id="d4e08-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[siteActivitySummary](../resources/siteactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e08-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e08-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4e08-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d4e08-154">CSV</span><span class="sxs-lookup"><span data-stu-id="d4e08-154">CSV</span></span>

<span data-ttu-id="d4e08-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d4e08-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d4e08-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e08-156">Request</span></span>

<span data-ttu-id="d4e08-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e08-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d4e08-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e08-158">Response</span></span>

<span data-ttu-id="d4e08-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e08-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d4e08-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d4e08-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="d4e08-161">JSON</span><span class="sxs-lookup"><span data-stu-id="d4e08-161">JSON</span></span>

<span data-ttu-id="d4e08-162">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e08-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d4e08-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e08-163">Request</span></span>

<span data-ttu-id="d4e08-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e08-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d4e08-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e08-165">Response</span></span>

<span data-ttu-id="d4e08-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e08-166">The following is an example of the response.</span></span>

> <span data-ttu-id="d4e08-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4e08-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
