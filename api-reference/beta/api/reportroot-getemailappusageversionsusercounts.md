---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ee00c3de308e6f1abfc9ccb6bb1457576212b67b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869201"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="3e0be-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="3e0be-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e0be-104">Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="3e0be-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="3e0be-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="3e0be-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e0be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e0be-106">Permissions</span></span>

<span data-ttu-id="3e0be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e0be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e0be-109">Permission type</span></span>                        | <span data-ttu-id="3e0be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e0be-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3e0be-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e0be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e0be-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e0be-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3e0be-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e0be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e0be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e0be-114">Not supported.</span></span>                           |
| <span data-ttu-id="3e0be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e0be-115">Application</span></span>                            | <span data-ttu-id="3e0be-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e0be-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="3e0be-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="3e0be-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3e0be-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3e0be-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e0be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0be-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3e0be-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3e0be-120">Function parameters</span></span>

<span data-ttu-id="3e0be-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3e0be-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3e0be-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3e0be-122">Parameter</span></span> | <span data-ttu-id="3e0be-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e0be-123">Type</span></span>   | <span data-ttu-id="3e0be-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e0be-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3e0be-125">ponto</span><span class="sxs-lookup"><span data-stu-id="3e0be-125">period</span></span>    | <span data-ttu-id="3e0be-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e0be-126">string</span></span> | <span data-ttu-id="3e0be-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3e0be-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3e0be-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3e0be-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3e0be-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3e0be-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3e0be-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e0be-130">Required.</span></span> |

<span data-ttu-id="3e0be-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3e0be-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="3e0be-132">The default output type is text/csv.</span></span> <span data-ttu-id="3e0be-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="3e0be-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e0be-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0be-134">Request headers</span></span>

| <span data-ttu-id="3e0be-135">Nome</span><span class="sxs-lookup"><span data-stu-id="3e0be-135">Name</span></span>          | <span data-ttu-id="3e0be-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e0be-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3e0be-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e0be-137">Authorization</span></span> | <span data-ttu-id="3e0be-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e0be-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3e0be-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0be-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3e0be-141">CSV</span><span class="sxs-lookup"><span data-stu-id="3e0be-141">CSV</span></span>

<span data-ttu-id="3e0be-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3e0be-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3e0be-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3e0be-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3e0be-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3e0be-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3e0be-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3e0be-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3e0be-146">Report Refresh Date</span></span>
- <span data-ttu-id="3e0be-147">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="3e0be-147">Outlook 2016</span></span>
- <span data-ttu-id="3e0be-148">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="3e0be-148">Outlook 2013</span></span>
- <span data-ttu-id="3e0be-149">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="3e0be-149">Outlook 2010</span></span>
- <span data-ttu-id="3e0be-150">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="3e0be-150">Outlook 2007</span></span>
- <span data-ttu-id="3e0be-151">Indefinido</span><span class="sxs-lookup"><span data-stu-id="3e0be-151">Undetermined</span></span>
- <span data-ttu-id="3e0be-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3e0be-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3e0be-153">JSON</span><span class="sxs-lookup"><span data-stu-id="3e0be-153">JSON</span></span>

<span data-ttu-id="3e0be-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-154">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e0be-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e0be-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3e0be-156">CSV</span><span class="sxs-lookup"><span data-stu-id="3e0be-156">CSV</span></span>

<span data-ttu-id="3e0be-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="3e0be-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3e0be-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0be-158">Request</span></span>

<span data-ttu-id="3e0be-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e0be-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3e0be-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0be-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e0be-161">C#</span><span class="sxs-lookup"><span data-stu-id="3e0be-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e0be-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e0be-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e0be-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e0be-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3e0be-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0be-164">Response</span></span>

<span data-ttu-id="3e0be-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3e0be-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3e0be-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="3e0be-167">JSON</span><span class="sxs-lookup"><span data-stu-id="3e0be-167">JSON</span></span>

<span data-ttu-id="3e0be-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="3e0be-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3e0be-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0be-169">Request</span></span>

<span data-ttu-id="3e0be-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e0be-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3e0be-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0be-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e0be-172">C#</span><span class="sxs-lookup"><span data-stu-id="3e0be-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e0be-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e0be-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e0be-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e0be-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3e0be-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0be-175">Response</span></span>

<span data-ttu-id="3e0be-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-176">The following is an example of the response.</span></span>

> <span data-ttu-id="3e0be-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e0be-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
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
