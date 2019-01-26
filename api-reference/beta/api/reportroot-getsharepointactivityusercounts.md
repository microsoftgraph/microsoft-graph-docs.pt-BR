---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 15734e15cf13cbbc03fd136d51bbdf9f4ac13ba0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573715"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="6b04a-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6b04a-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b04a-105">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="6b04a-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="6b04a-106">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="6b04a-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="6b04a-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="6b04a-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b04a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b04a-108">Permissions</span></span>

<span data-ttu-id="6b04a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b04a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b04a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b04a-111">Permission type</span></span>                        | <span data-ttu-id="6b04a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b04a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6b04a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b04a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b04a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b04a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6b04a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b04a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b04a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b04a-116">Not supported.</span></span>                           |
| <span data-ttu-id="6b04a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b04a-117">Application</span></span>                            | <span data-ttu-id="6b04a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b04a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6b04a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b04a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6b04a-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6b04a-120">Function parameters</span></span>

<span data-ttu-id="6b04a-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6b04a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6b04a-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6b04a-122">Parameter</span></span> | <span data-ttu-id="6b04a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b04a-123">Type</span></span>   | <span data-ttu-id="6b04a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b04a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6b04a-125">ponto</span><span class="sxs-lookup"><span data-stu-id="6b04a-125">period</span></span>    | <span data-ttu-id="6b04a-126">string</span><span class="sxs-lookup"><span data-stu-id="6b04a-126">string</span></span> | <span data-ttu-id="6b04a-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6b04a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6b04a-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6b04a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6b04a-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6b04a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6b04a-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b04a-130">Required.</span></span> |

<span data-ttu-id="6b04a-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b04a-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6b04a-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="6b04a-132">The default output type is text/csv.</span></span> <span data-ttu-id="6b04a-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="6b04a-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b04a-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b04a-134">Request headers</span></span>

| <span data-ttu-id="6b04a-135">Nome</span><span class="sxs-lookup"><span data-stu-id="6b04a-135">Name</span></span>          | <span data-ttu-id="6b04a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b04a-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6b04a-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b04a-137">Authorization</span></span> | <span data-ttu-id="6b04a-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b04a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6b04a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b04a-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6b04a-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6b04a-141">CSV</span></span>

<span data-ttu-id="6b04a-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6b04a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6b04a-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6b04a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6b04a-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6b04a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6b04a-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6b04a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6b04a-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6b04a-146">Report Refresh Date</span></span>
- <span data-ttu-id="6b04a-147">Página visitada</span><span class="sxs-lookup"><span data-stu-id="6b04a-147">Visited Page</span></span>
- <span data-ttu-id="6b04a-148">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="6b04a-148">Viewed Or Edited</span></span>
- <span data-ttu-id="6b04a-149">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="6b04a-149">Synced</span></span>
- <span data-ttu-id="6b04a-150">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="6b04a-150">Shared Internally</span></span>
- <span data-ttu-id="6b04a-151">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="6b04a-151">Shared Externally</span></span>
- <span data-ttu-id="6b04a-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="6b04a-152">Report Date</span></span>
- <span data-ttu-id="6b04a-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6b04a-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6b04a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="6b04a-154">JSON</span></span>

<span data-ttu-id="6b04a-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b04a-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b04a-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b04a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6b04a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="6b04a-157">CSV</span></span>

<span data-ttu-id="6b04a-158">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="6b04a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6b04a-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b04a-159">Request</span></span>

<span data-ttu-id="6b04a-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b04a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6b04a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b04a-161">Response</span></span>

<span data-ttu-id="6b04a-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b04a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6b04a-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6b04a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="6b04a-164">JSON</span><span class="sxs-lookup"><span data-stu-id="6b04a-164">JSON</span></span>

<span data-ttu-id="6b04a-165">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="6b04a-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6b04a-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b04a-166">Request</span></span>

<span data-ttu-id="6b04a-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b04a-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6b04a-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b04a-168">Response</span></span>

<span data-ttu-id="6b04a-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b04a-169">The following is an example of the response.</span></span>

> <span data-ttu-id="6b04a-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b04a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
