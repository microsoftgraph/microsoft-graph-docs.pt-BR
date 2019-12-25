---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d92293e3daba5ba86d18ecdea347d70782e13170
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867551"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="db5cd-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="db5cd-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db5cd-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="db5cd-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="db5cd-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="db5cd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="db5cd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db5cd-106">Permissions</span></span>

<span data-ttu-id="db5cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db5cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db5cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db5cd-109">Permission type</span></span>                        | <span data-ttu-id="db5cd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db5cd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="db5cd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db5cd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db5cd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5cd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="db5cd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db5cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db5cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db5cd-114">Not supported.</span></span>                           |
| <span data-ttu-id="db5cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db5cd-115">Application</span></span>                            | <span data-ttu-id="db5cd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db5cd-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="db5cd-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="db5cd-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="db5cd-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="db5cd-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="db5cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db5cd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="db5cd-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="db5cd-120">Function parameters</span></span>

<span data-ttu-id="db5cd-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="db5cd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="db5cd-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="db5cd-122">Parameter</span></span> | <span data-ttu-id="db5cd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="db5cd-123">Type</span></span>   | <span data-ttu-id="db5cd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="db5cd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="db5cd-125">ponto</span><span class="sxs-lookup"><span data-stu-id="db5cd-125">period</span></span>    | <span data-ttu-id="db5cd-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db5cd-126">string</span></span> | <span data-ttu-id="db5cd-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="db5cd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="db5cd-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="db5cd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="db5cd-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="db5cd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="db5cd-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db5cd-130">Required.</span></span> |

<span data-ttu-id="db5cd-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="db5cd-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="db5cd-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="db5cd-132">The default output type is text/csv.</span></span> <span data-ttu-id="db5cd-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="db5cd-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db5cd-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db5cd-134">Request headers</span></span>

| <span data-ttu-id="db5cd-135">Nome</span><span class="sxs-lookup"><span data-stu-id="db5cd-135">Name</span></span>          | <span data-ttu-id="db5cd-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="db5cd-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="db5cd-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="db5cd-137">Authorization</span></span> | <span data-ttu-id="db5cd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db5cd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="db5cd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="db5cd-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="db5cd-141">CSV</span><span class="sxs-lookup"><span data-stu-id="db5cd-141">CSV</span></span>

<span data-ttu-id="db5cd-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="db5cd-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="db5cd-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="db5cd-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="db5cd-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="db5cd-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="db5cd-145">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="db5cd-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="db5cd-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="db5cd-146">Report Refresh Date</span></span>
- <span data-ttu-id="db5cd-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="db5cd-147">Office 365</span></span>
- <span data-ttu-id="db5cd-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="db5cd-148">Exchange</span></span>
- <span data-ttu-id="db5cd-149">OneDrive</span><span class="sxs-lookup"><span data-stu-id="db5cd-149">OneDrive</span></span>
- <span data-ttu-id="db5cd-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="db5cd-150">SharePoint</span></span>
- <span data-ttu-id="db5cd-151">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="db5cd-151">Skype For Business</span></span> 
- <span data-ttu-id="db5cd-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="db5cd-152">Yammer</span></span>
- <span data-ttu-id="db5cd-153">Teams</span><span class="sxs-lookup"><span data-stu-id="db5cd-153">Teams</span></span>
- <span data-ttu-id="db5cd-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="db5cd-154">Report Date</span></span>
- <span data-ttu-id="db5cd-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="db5cd-155">Report Period</span></span>

<span data-ttu-id="db5cd-156">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="db5cd-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="db5cd-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="db5cd-157">Yammer</span></span>
- <span data-ttu-id="db5cd-158">Teams</span><span class="sxs-lookup"><span data-stu-id="db5cd-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="db5cd-159">JSON</span><span class="sxs-lookup"><span data-stu-id="db5cd-159">JSON</span></span>

<span data-ttu-id="db5cd-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db5cd-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="db5cd-161">As propriedades a seguir no objeto **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="db5cd-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="db5cd-162">Yammer</span><span class="sxs-lookup"><span data-stu-id="db5cd-162">yammer</span></span>
- <span data-ttu-id="db5cd-163">Teams</span><span class="sxs-lookup"><span data-stu-id="db5cd-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="db5cd-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db5cd-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="db5cd-165">CSV</span><span class="sxs-lookup"><span data-stu-id="db5cd-165">CSV</span></span>

<span data-ttu-id="db5cd-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="db5cd-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="db5cd-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db5cd-167">Request</span></span>

<span data-ttu-id="db5cd-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db5cd-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db5cd-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="db5cd-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db5cd-170">C#</span><span class="sxs-lookup"><span data-stu-id="db5cd-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db5cd-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db5cd-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db5cd-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db5cd-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db5cd-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="db5cd-173">Response</span></span>

<span data-ttu-id="db5cd-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db5cd-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="db5cd-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="db5cd-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="db5cd-176">JSON</span><span class="sxs-lookup"><span data-stu-id="db5cd-176">JSON</span></span>

<span data-ttu-id="db5cd-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="db5cd-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="db5cd-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db5cd-178">Request</span></span>

<span data-ttu-id="db5cd-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db5cd-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db5cd-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="db5cd-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db5cd-181">C#</span><span class="sxs-lookup"><span data-stu-id="db5cd-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db5cd-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db5cd-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db5cd-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db5cd-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db5cd-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="db5cd-184">Response</span></span>

<span data-ttu-id="db5cd-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db5cd-185">The following is an example of the response.</span></span>

> <span data-ttu-id="db5cd-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db5cd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
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
