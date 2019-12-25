---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f9f117cb11280d573076cf9a7278c96f4f4e6dbe
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869105"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="5a44a-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="5a44a-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a44a-104">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="5a44a-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="5a44a-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="5a44a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a44a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a44a-106">Permissions</span></span>

<span data-ttu-id="5a44a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a44a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a44a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a44a-109">Permission type</span></span>                        | <span data-ttu-id="5a44a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a44a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5a44a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a44a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a44a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a44a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5a44a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a44a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a44a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a44a-114">Not supported.</span></span>                           |
| <span data-ttu-id="5a44a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-115">Application</span></span>                            | <span data-ttu-id="5a44a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a44a-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="5a44a-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="5a44a-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5a44a-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5a44a-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5a44a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a44a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5a44a-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5a44a-120">Function parameters</span></span>

<span data-ttu-id="5a44a-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5a44a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5a44a-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5a44a-122">Parameter</span></span> | <span data-ttu-id="5a44a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a44a-123">Type</span></span>   | <span data-ttu-id="5a44a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a44a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5a44a-125">ponto</span><span class="sxs-lookup"><span data-stu-id="5a44a-125">period</span></span>    | <span data-ttu-id="5a44a-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a44a-126">string</span></span> | <span data-ttu-id="5a44a-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5a44a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5a44a-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5a44a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5a44a-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5a44a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5a44a-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a44a-130">Required.</span></span> |

<span data-ttu-id="5a44a-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a44a-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5a44a-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="5a44a-132">The default output type is text/csv.</span></span> <span data-ttu-id="5a44a-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5a44a-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a44a-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a44a-134">Request headers</span></span>

| <span data-ttu-id="5a44a-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5a44a-135">Name</span></span>          | <span data-ttu-id="5a44a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a44a-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5a44a-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a44a-137">Authorization</span></span> | <span data-ttu-id="5a44a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a44a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5a44a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a44a-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5a44a-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5a44a-141">CSV</span></span>

<span data-ttu-id="5a44a-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5a44a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5a44a-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5a44a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5a44a-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5a44a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5a44a-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5a44a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5a44a-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5a44a-146">Report Refresh Date</span></span>
- <span data-ttu-id="5a44a-147">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-147">Exchange Active</span></span>
- <span data-ttu-id="5a44a-148">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-148">Exchange Inactive</span></span>
- <span data-ttu-id="5a44a-149">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-149">OneDrive Active</span></span>
- <span data-ttu-id="5a44a-150">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-150">OneDrive Inactive</span></span>
- <span data-ttu-id="5a44a-151">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-151">SharePoint Active</span></span>
- <span data-ttu-id="5a44a-152">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-152">SharePoint Inactive</span></span>
- <span data-ttu-id="5a44a-153">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-153">Skype For Business Active</span></span>
- <span data-ttu-id="5a44a-154">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="5a44a-155">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="5a44a-155">Yammer Active</span></span>
- <span data-ttu-id="5a44a-156">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="5a44a-156">Yammer Inactive</span></span>
- <span data-ttu-id="5a44a-157">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-157">Teams Active</span></span>
- <span data-ttu-id="5a44a-158">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-158">Teams Inactive</span></span>
- <span data-ttu-id="5a44a-159">Office 365 active</span><span class="sxs-lookup"><span data-stu-id="5a44a-159">Office 365 Active</span></span>
- <span data-ttu-id="5a44a-160">Office 365 inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-160">Office 365 Inactive</span></span>
- <span data-ttu-id="5a44a-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5a44a-161">Report Period</span></span>

<span data-ttu-id="5a44a-162">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="5a44a-162">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5a44a-163">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="5a44a-163">Yammer Active</span></span>
- <span data-ttu-id="5a44a-164">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="5a44a-164">Yammer Inactive</span></span>
- <span data-ttu-id="5a44a-165">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-165">Teams Active</span></span>
- <span data-ttu-id="5a44a-166">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="5a44a-166">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="5a44a-167">JSON</span><span class="sxs-lookup"><span data-stu-id="5a44a-167">JSON</span></span>

<span data-ttu-id="5a44a-168">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a44a-168">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="5a44a-169">As propriedades a seguir no objeto **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="5a44a-169">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5a44a-170">yammerActive</span><span class="sxs-lookup"><span data-stu-id="5a44a-170">yammerActive</span></span>
- <span data-ttu-id="5a44a-171">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="5a44a-171">yammerInactive</span></span>
- <span data-ttu-id="5a44a-172">teamsActive</span><span class="sxs-lookup"><span data-stu-id="5a44a-172">teamsActive</span></span>
- <span data-ttu-id="5a44a-173">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="5a44a-173">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="5a44a-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a44a-174">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5a44a-175">CSV</span><span class="sxs-lookup"><span data-stu-id="5a44a-175">CSV</span></span>

<span data-ttu-id="5a44a-176">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="5a44a-176">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5a44a-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a44a-177">Request</span></span>

<span data-ttu-id="5a44a-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a44a-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5a44a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a44a-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a44a-180">C#</span><span class="sxs-lookup"><span data-stu-id="5a44a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a44a-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a44a-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a44a-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a44a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a44a-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a44a-183">Response</span></span>

<span data-ttu-id="5a44a-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a44a-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5a44a-185">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5a44a-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="5a44a-186">JSON</span><span class="sxs-lookup"><span data-stu-id="5a44a-186">JSON</span></span> 

<span data-ttu-id="5a44a-187">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5a44a-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5a44a-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a44a-188">Request</span></span>

<span data-ttu-id="5a44a-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a44a-189">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5a44a-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a44a-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a44a-191">C#</span><span class="sxs-lookup"><span data-stu-id="5a44a-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a44a-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a44a-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a44a-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a44a-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a44a-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a44a-194">Response</span></span>

<span data-ttu-id="5a44a-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a44a-195">The following is an example of the response.</span></span>

> <span data-ttu-id="5a44a-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a44a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "office365Active": 2791,
      "office365Inactive": 503,
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
