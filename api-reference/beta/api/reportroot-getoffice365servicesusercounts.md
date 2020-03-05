---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7b1f7f09d28a9df5d2f6d9386c7372e81ae315af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454336"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="94287-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="94287-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="94287-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94287-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94287-105">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="94287-105">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="94287-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="94287-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="94287-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94287-107">Permissions</span></span>

<span data-ttu-id="94287-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94287-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94287-110">Permission type</span></span>                        | <span data-ttu-id="94287-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94287-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="94287-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94287-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94287-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94287-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="94287-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94287-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94287-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94287-115">Not supported.</span></span>                           |
| <span data-ttu-id="94287-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94287-116">Application</span></span>                            | <span data-ttu-id="94287-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94287-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="94287-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="94287-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="94287-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="94287-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="94287-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94287-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="94287-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="94287-121">Function parameters</span></span>

<span data-ttu-id="94287-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="94287-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="94287-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94287-123">Parameter</span></span> | <span data-ttu-id="94287-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="94287-124">Type</span></span>   | <span data-ttu-id="94287-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="94287-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="94287-126">ponto</span><span class="sxs-lookup"><span data-stu-id="94287-126">period</span></span>    | <span data-ttu-id="94287-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94287-127">string</span></span> | <span data-ttu-id="94287-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="94287-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="94287-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="94287-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="94287-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="94287-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="94287-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94287-131">Required.</span></span> |

<span data-ttu-id="94287-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94287-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="94287-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="94287-133">The default output type is text/csv.</span></span> <span data-ttu-id="94287-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="94287-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94287-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94287-135">Request headers</span></span>

| <span data-ttu-id="94287-136">Nome</span><span class="sxs-lookup"><span data-stu-id="94287-136">Name</span></span>          | <span data-ttu-id="94287-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="94287-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="94287-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="94287-138">Authorization</span></span> | <span data-ttu-id="94287-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94287-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="94287-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="94287-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="94287-142">CSV</span><span class="sxs-lookup"><span data-stu-id="94287-142">CSV</span></span>

<span data-ttu-id="94287-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="94287-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="94287-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="94287-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="94287-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="94287-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="94287-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="94287-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="94287-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="94287-147">Report Refresh Date</span></span>
- <span data-ttu-id="94287-148">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="94287-148">Exchange Active</span></span>
- <span data-ttu-id="94287-149">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="94287-149">Exchange Inactive</span></span>
- <span data-ttu-id="94287-150">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="94287-150">OneDrive Active</span></span>
- <span data-ttu-id="94287-151">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="94287-151">OneDrive Inactive</span></span>
- <span data-ttu-id="94287-152">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="94287-152">SharePoint Active</span></span>
- <span data-ttu-id="94287-153">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="94287-153">SharePoint Inactive</span></span>
- <span data-ttu-id="94287-154">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="94287-154">Skype For Business Active</span></span>
- <span data-ttu-id="94287-155">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="94287-155">Skype For Business Inactive</span></span>
- <span data-ttu-id="94287-156">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="94287-156">Yammer Active</span></span>
- <span data-ttu-id="94287-157">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="94287-157">Yammer Inactive</span></span>
- <span data-ttu-id="94287-158">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="94287-158">Teams Active</span></span>
- <span data-ttu-id="94287-159">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="94287-159">Teams Inactive</span></span>
- <span data-ttu-id="94287-160">Office 365 active</span><span class="sxs-lookup"><span data-stu-id="94287-160">Office 365 Active</span></span>
- <span data-ttu-id="94287-161">Office 365 inativo</span><span class="sxs-lookup"><span data-stu-id="94287-161">Office 365 Inactive</span></span>
- <span data-ttu-id="94287-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="94287-162">Report Period</span></span>

<span data-ttu-id="94287-163">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="94287-163">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="94287-164">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="94287-164">Yammer Active</span></span>
- <span data-ttu-id="94287-165">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="94287-165">Yammer Inactive</span></span>
- <span data-ttu-id="94287-166">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="94287-166">Teams Active</span></span>
- <span data-ttu-id="94287-167">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="94287-167">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="94287-168">JSON</span><span class="sxs-lookup"><span data-stu-id="94287-168">JSON</span></span>

<span data-ttu-id="94287-169">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94287-169">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="94287-170">As propriedades a seguir no objeto **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="94287-170">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="94287-171">yammerActive</span><span class="sxs-lookup"><span data-stu-id="94287-171">yammerActive</span></span>
- <span data-ttu-id="94287-172">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="94287-172">yammerInactive</span></span>
- <span data-ttu-id="94287-173">teamsActive</span><span class="sxs-lookup"><span data-stu-id="94287-173">teamsActive</span></span>
- <span data-ttu-id="94287-174">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="94287-174">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="94287-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94287-175">Example</span></span>

### <a name="csv"></a><span data-ttu-id="94287-176">CSV</span><span class="sxs-lookup"><span data-stu-id="94287-176">CSV</span></span>

<span data-ttu-id="94287-177">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="94287-177">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="94287-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94287-178">Request</span></span>

<span data-ttu-id="94287-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94287-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94287-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="94287-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="94287-181">C#</span><span class="sxs-lookup"><span data-stu-id="94287-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94287-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94287-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94287-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94287-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94287-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="94287-184">Response</span></span>

<span data-ttu-id="94287-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94287-185">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="94287-186">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="94287-186">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="94287-187">JSON</span><span class="sxs-lookup"><span data-stu-id="94287-187">JSON</span></span> 

<span data-ttu-id="94287-188">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="94287-188">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="94287-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94287-189">Request</span></span>

<span data-ttu-id="94287-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94287-190">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94287-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="94287-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="94287-192">C#</span><span class="sxs-lookup"><span data-stu-id="94287-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94287-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94287-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94287-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94287-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94287-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="94287-195">Response</span></span>

<span data-ttu-id="94287-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94287-196">The following is an example of the response.</span></span>

> <span data-ttu-id="94287-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94287-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
