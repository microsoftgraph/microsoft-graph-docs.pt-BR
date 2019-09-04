---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 97347fc7884228fb60d1964f64624607d1074de8
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723011"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="f9913-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="f9913-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9913-104">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f9913-104">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="f9913-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="f9913-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9913-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9913-106">Permissions</span></span>

<span data-ttu-id="f9913-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9913-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9913-109">Permission type</span></span>                        | <span data-ttu-id="f9913-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9913-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f9913-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9913-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9913-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9913-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f9913-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9913-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9913-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9913-114">Not supported.</span></span>                           |
| <span data-ttu-id="f9913-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9913-115">Application</span></span>                            | <span data-ttu-id="f9913-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9913-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f9913-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9913-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f9913-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f9913-118">Function parameters</span></span>

<span data-ttu-id="f9913-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f9913-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f9913-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9913-120">Parameter</span></span> | <span data-ttu-id="f9913-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9913-121">Type</span></span>   | <span data-ttu-id="f9913-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9913-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f9913-123">ponto</span><span class="sxs-lookup"><span data-stu-id="f9913-123">period</span></span>    | <span data-ttu-id="f9913-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9913-124">string</span></span> | <span data-ttu-id="f9913-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f9913-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f9913-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f9913-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f9913-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f9913-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f9913-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9913-128">Required.</span></span> |

<span data-ttu-id="f9913-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9913-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f9913-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="f9913-130">The default output type is text/csv.</span></span> <span data-ttu-id="f9913-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="f9913-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9913-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9913-132">Request headers</span></span>

| <span data-ttu-id="f9913-133">Nome</span><span class="sxs-lookup"><span data-stu-id="f9913-133">Name</span></span>          | <span data-ttu-id="f9913-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9913-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f9913-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9913-135">Authorization</span></span> | <span data-ttu-id="f9913-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9913-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f9913-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9913-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f9913-139">CSV</span><span class="sxs-lookup"><span data-stu-id="f9913-139">CSV</span></span>

<span data-ttu-id="f9913-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f9913-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f9913-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f9913-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f9913-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f9913-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f9913-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f9913-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f9913-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f9913-144">Report Refresh Date</span></span>
- <span data-ttu-id="f9913-145">Total</span><span class="sxs-lookup"><span data-stu-id="f9913-145">Total</span></span>
- <span data-ttu-id="f9913-146">Ativo</span><span class="sxs-lookup"><span data-stu-id="f9913-146">Active</span></span>
- <span data-ttu-id="f9913-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="f9913-147">Report Date</span></span>
- <span data-ttu-id="f9913-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f9913-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f9913-149">JSON</span><span class="sxs-lookup"><span data-stu-id="f9913-149">JSON</span></span>

<span data-ttu-id="f9913-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9913-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9913-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9913-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f9913-152">CSV</span><span class="sxs-lookup"><span data-stu-id="f9913-152">CSV</span></span>

<span data-ttu-id="f9913-153">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="f9913-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f9913-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9913-154">Request</span></span>

<span data-ttu-id="f9913-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9913-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9913-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9913-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9913-157">C#</span><span class="sxs-lookup"><span data-stu-id="f9913-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitygroupcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9913-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9913-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitygroupcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9913-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f9913-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitygroupcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9913-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9913-160">Response</span></span>

<span data-ttu-id="f9913-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9913-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f9913-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f9913-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f9913-163">JSON</span><span class="sxs-lookup"><span data-stu-id="f9913-163">JSON</span></span>

<span data-ttu-id="f9913-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="f9913-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f9913-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9913-165">Request</span></span>

<span data-ttu-id="f9913-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9913-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9913-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9913-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9913-168">C#</span><span class="sxs-lookup"><span data-stu-id="f9913-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitygroupcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9913-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9913-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitygroupcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9913-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f9913-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitygroupcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9913-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9913-171">Response</span></span>

<span data-ttu-id="f9913-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9913-172">The following is an example of the response.</span></span>

> <span data-ttu-id="f9913-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9913-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
