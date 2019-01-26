---
title: 'reportRoot: getSharePointActivityPages'
description: Obtenha o número de páginas exclusivas visitadas pelos usuários.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 223e7718e86102c7cddd0a5211ac176434cd540c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576847"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="becca-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="becca-103">reportRoot: getSharePointActivityPages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="becca-104">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="becca-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="becca-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="becca-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="becca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="becca-106">Permissions</span></span>

<span data-ttu-id="becca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="becca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="becca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="becca-109">Permission type</span></span>                        | <span data-ttu-id="becca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="becca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="becca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="becca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="becca-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="becca-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="becca-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="becca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="becca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="becca-114">Not supported.</span></span>                           |
| <span data-ttu-id="becca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="becca-115">Application</span></span>                            | <span data-ttu-id="becca-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="becca-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="becca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="becca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="becca-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="becca-118">Function parameters</span></span>

<span data-ttu-id="becca-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="becca-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="becca-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="becca-120">Parameter</span></span> | <span data-ttu-id="becca-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="becca-121">Type</span></span>   | <span data-ttu-id="becca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="becca-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="becca-123">ponto</span><span class="sxs-lookup"><span data-stu-id="becca-123">period</span></span>    | <span data-ttu-id="becca-124">string</span><span class="sxs-lookup"><span data-stu-id="becca-124">string</span></span> | <span data-ttu-id="becca-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="becca-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="becca-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="becca-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="becca-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="becca-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="becca-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="becca-128">Required.</span></span> |

<span data-ttu-id="becca-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="becca-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="becca-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="becca-130">The default output type is text/csv.</span></span> <span data-ttu-id="becca-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="becca-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="becca-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="becca-132">Request headers</span></span>

| <span data-ttu-id="becca-133">Nome</span><span class="sxs-lookup"><span data-stu-id="becca-133">Name</span></span>          | <span data-ttu-id="becca-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="becca-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="becca-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="becca-135">Authorization</span></span> | <span data-ttu-id="becca-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="becca-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="becca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="becca-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="becca-139">CSV</span><span class="sxs-lookup"><span data-stu-id="becca-139">CSV</span></span>

<span data-ttu-id="becca-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="becca-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="becca-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="becca-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="becca-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="becca-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="becca-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="becca-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="becca-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="becca-144">Report Refresh Date</span></span>
- <span data-ttu-id="becca-145">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="becca-145">Visited Page Count</span></span>
- <span data-ttu-id="becca-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="becca-146">Report Date</span></span>
- <span data-ttu-id="becca-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="becca-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="becca-148">JSON</span><span class="sxs-lookup"><span data-stu-id="becca-148">JSON</span></span>

<span data-ttu-id="becca-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointActivityPages](../resources/sharepointactivitypages.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="becca-149">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="becca-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="becca-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="becca-151">CSV</span><span class="sxs-lookup"><span data-stu-id="becca-151">CSV</span></span>

<span data-ttu-id="becca-152">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="becca-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="becca-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="becca-153">Request</span></span>

<span data-ttu-id="becca-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="becca-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="becca-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="becca-155">Response</span></span>

<span data-ttu-id="becca-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="becca-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="becca-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="becca-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="becca-158">JSON</span><span class="sxs-lookup"><span data-stu-id="becca-158">JSON</span></span>

<span data-ttu-id="becca-159">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="becca-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="becca-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="becca-160">Request</span></span>

<span data-ttu-id="becca-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="becca-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="becca-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="becca-162">Response</span></span>

<span data-ttu-id="becca-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="becca-163">The following is an example of the response.</span></span>

> <span data-ttu-id="becca-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="becca-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivitypages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
