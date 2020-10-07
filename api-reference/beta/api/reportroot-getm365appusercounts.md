---
title: 'reportRoot: getM365AppUserCounts'
description: Obter um relatório que fornece a tendência no número de usuários ativos para cada aplicativo – Outlook, Word, Excel, PowerPoint, OneNote e equipes – em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1012941b4f39af4b3f26ee0ae0eef60dfcaf4898
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373731"
---
# <a name="reportroot-getm365appusercounts"></a><span data-ttu-id="bda6b-103">reportRoot: getM365AppUserCounts</span><span class="sxs-lookup"><span data-stu-id="bda6b-103">reportRoot: getM365AppUserCounts</span></span>

<span data-ttu-id="bda6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda6b-105">Obter um relatório que fornece a tendência no número de usuários ativos para cada aplicativo – Outlook, Word, Excel, PowerPoint, OneNote e equipes – em sua organização.</span><span class="sxs-lookup"><span data-stu-id="bda6b-105">Get a report that provides the trend in the number of active users for each app – Outlook, Word, Excel, PowerPoint, OneNote, and Teams - in your organization.</span></span>

> <span data-ttu-id="bda6b-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-microsoft 365 apps Usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span><span class="sxs-lookup"><span data-stu-id="bda6b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="bda6b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bda6b-107">Permissions</span></span>

<span data-ttu-id="bda6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bda6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bda6b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bda6b-110">Permission type</span></span>                        | <span data-ttu-id="bda6b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bda6b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bda6b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bda6b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bda6b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bda6b-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="bda6b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bda6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bda6b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bda6b-115">Not supported.</span></span>                              |
| <span data-ttu-id="bda6b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bda6b-116">Application</span></span>                            | <span data-ttu-id="bda6b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bda6b-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="bda6b-118">**Observação:** Para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure AD apropriada.</span><span class="sxs-lookup"><span data-stu-id="bda6b-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="bda6b-119">Para obter detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="bda6b-119">For details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="bda6b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bda6b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bda6b-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bda6b-121">Function parameters</span></span>

<span data-ttu-id="bda6b-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bda6b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bda6b-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bda6b-123">Parameter</span></span> | <span data-ttu-id="bda6b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bda6b-124">Type</span></span>   | <span data-ttu-id="bda6b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bda6b-125">Description</span></span>                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bda6b-126">ponto</span><span class="sxs-lookup"><span data-stu-id="bda6b-126">period</span></span>    | <span data-ttu-id="bda6b-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bda6b-127">string</span></span> | <span data-ttu-id="bda6b-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bda6b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bda6b-129">Os valores com suporte para {period_value} são: `D7` , `D30` , `D90` , e `D180` .</span><span class="sxs-lookup"><span data-stu-id="bda6b-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="bda6b-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bda6b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bda6b-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bda6b-131">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="bda6b-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bda6b-132">Optional query parameters</span></span>

<span data-ttu-id="bda6b-133">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bda6b-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bda6b-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="bda6b-134">The default output type is text/csv.</span></span> <span data-ttu-id="bda6b-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o `$format` parâmetro de consulta OData para definir a saída padrão como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="bda6b-135">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bda6b-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bda6b-136">Request headers</span></span>

| <span data-ttu-id="bda6b-137">Nome</span><span class="sxs-lookup"><span data-stu-id="bda6b-137">Name</span></span>          | <span data-ttu-id="bda6b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="bda6b-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bda6b-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="bda6b-139">Authorization</span></span> | <span data-ttu-id="bda6b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bda6b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bda6b-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bda6b-142">Request body</span></span>

<span data-ttu-id="bda6b-143">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="bda6b-143">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="bda6b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bda6b-144">Response</span></span>

<span data-ttu-id="bda6b-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Report](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bda6b-145">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="bda6b-146">Os dados do relatório estão contidos na propriedade de **conteúdo** do objeto **Report** .</span><span class="sxs-lookup"><span data-stu-id="bda6b-146">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="bda6b-147">CSV</span><span class="sxs-lookup"><span data-stu-id="bda6b-147">CSV</span></span>

<span data-ttu-id="bda6b-148">Se tiver êxito, solicitar a propriedade **Content** retornará uma `302 Found` resposta que REDIRECIONA para uma URL de download autenticado para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bda6b-148">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bda6b-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bda6b-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bda6b-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bda6b-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bda6b-151">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="bda6b-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="bda6b-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bda6b-152">Report Refresh Date</span></span>
- <span data-ttu-id="bda6b-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bda6b-153">Report Period</span></span>
- <span data-ttu-id="bda6b-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="bda6b-154">Report Date</span></span>
- <span data-ttu-id="bda6b-155">Outlook</span><span class="sxs-lookup"><span data-stu-id="bda6b-155">Outlook</span></span>
- <span data-ttu-id="bda6b-156">Word</span><span class="sxs-lookup"><span data-stu-id="bda6b-156">Word</span></span>
- <span data-ttu-id="bda6b-157">Excel</span><span class="sxs-lookup"><span data-stu-id="bda6b-157">Excel</span></span>
- <span data-ttu-id="bda6b-158">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="bda6b-158">PowerPoint</span></span>
- <span data-ttu-id="bda6b-159">OneNote</span><span class="sxs-lookup"><span data-stu-id="bda6b-159">OneNote</span></span>
- <span data-ttu-id="bda6b-160">Teams</span><span class="sxs-lookup"><span data-stu-id="bda6b-160">Teams</span></span>

### <a name="json"></a><span data-ttu-id="bda6b-161">JSON</span><span class="sxs-lookup"><span data-stu-id="bda6b-161">JSON</span></span>

<span data-ttu-id="bda6b-162">Se bem-sucedido, solicitar a propriedade **Content** retorna um `200 OK` código de resposta e um objeto JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bda6b-162">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bda6b-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bda6b-163">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="bda6b-164">Exemplo 1: saída CSV</span><span class="sxs-lookup"><span data-stu-id="bda6b-164">Example 1: CSV output</span></span>

<span data-ttu-id="bda6b-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="bda6b-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bda6b-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bda6b-166">Request</span></span>

<span data-ttu-id="bda6b-167">Veja a seguir um exemplo da solicitação para obter a propriedade de **conteúdo** .</span><span class="sxs-lookup"><span data-stu-id="bda6b-167">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="bda6b-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="bda6b-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserCounts(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="bda6b-169">C#</span><span class="sxs-lookup"><span data-stu-id="bda6b-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bda6b-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bda6b-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bda6b-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bda6b-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="bda6b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="bda6b-172">Response</span></span>

<span data-ttu-id="bda6b-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bda6b-173">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bda6b-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bda6b-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Period,Report Date,Outlook,Word,Excel,PowerPoint,OneNote,Teams
```

### <a name="example-2-json-output"></a><span data-ttu-id="bda6b-175">Exemplo 2: saída JSON</span><span class="sxs-lookup"><span data-stu-id="bda6b-175">Example 2: JSON output</span></span>

<span data-ttu-id="bda6b-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="bda6b-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bda6b-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bda6b-177">Request</span></span>

<span data-ttu-id="bda6b-178">Veja a seguir um exemplo da solicitação para obter a propriedade de **conteúdo** .</span><span class="sxs-lookup"><span data-stu-id="bda6b-178">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="bda6b-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="bda6b-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserCounts(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="bda6b-180">C#</span><span class="sxs-lookup"><span data-stu-id="bda6b-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bda6b-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bda6b-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bda6b-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bda6b-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="bda6b-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="bda6b-183">Response</span></span>

<span data-ttu-id="bda6b-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bda6b-184">The following is an example of the response.</span></span>

> <span data-ttu-id="bda6b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bda6b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "reportPeriod": 7,
      "userCounts": [
        {
          "reportDate": "2020-06-30",
          "outlook": 1513,
          "word": 911,
          "excel": 790,
          "powerPoint": 683,
          "oneNote": 969,
          "teams": 1532
        }
      ]
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
