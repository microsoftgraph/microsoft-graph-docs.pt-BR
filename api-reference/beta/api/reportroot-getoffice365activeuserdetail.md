---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ba73993ffdf205e197058afa2d9aea2648e7c877
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518146"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="70000-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="70000-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70000-104">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="70000-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="70000-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="70000-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="70000-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="70000-106">Permissions</span></span>

<span data-ttu-id="70000-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70000-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70000-109">Permission type</span></span>                        | <span data-ttu-id="70000-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70000-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70000-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70000-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70000-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70000-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="70000-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70000-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70000-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70000-114">Not supported.</span></span>                           |
| <span data-ttu-id="70000-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70000-115">Application</span></span>                            | <span data-ttu-id="70000-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70000-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="70000-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70000-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="70000-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="70000-118">Function parameters</span></span>

<span data-ttu-id="70000-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="70000-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="70000-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="70000-120">Parameter</span></span> | <span data-ttu-id="70000-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="70000-121">Type</span></span>   | <span data-ttu-id="70000-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="70000-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70000-123">ponto</span><span class="sxs-lookup"><span data-stu-id="70000-123">period</span></span>    | <span data-ttu-id="70000-124">string</span><span class="sxs-lookup"><span data-stu-id="70000-124">string</span></span> | <span data-ttu-id="70000-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="70000-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70000-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="70000-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70000-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="70000-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="70000-128">data</span><span class="sxs-lookup"><span data-stu-id="70000-128">date</span></span>      | <span data-ttu-id="70000-129">Data</span><span class="sxs-lookup"><span data-stu-id="70000-129">Date</span></span>   | <span data-ttu-id="70000-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="70000-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="70000-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="70000-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="70000-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="70000-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="70000-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="70000-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="70000-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="70000-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="70000-135">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="70000-135">The default output type is text/csv.</span></span> <span data-ttu-id="70000-136">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="70000-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70000-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70000-137">Request headers</span></span>

| <span data-ttu-id="70000-138">Nome</span><span class="sxs-lookup"><span data-stu-id="70000-138">Name</span></span>          | <span data-ttu-id="70000-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="70000-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="70000-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="70000-140">Authorization</span></span> | <span data-ttu-id="70000-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70000-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="70000-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="70000-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="70000-144">CSV</span><span class="sxs-lookup"><span data-stu-id="70000-144">CSV</span></span>

<span data-ttu-id="70000-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="70000-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70000-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="70000-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70000-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="70000-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70000-148">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="70000-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="70000-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="70000-149">Report Refresh Date</span></span>
- <span data-ttu-id="70000-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="70000-150">User Principal Name</span></span>
- <span data-ttu-id="70000-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="70000-151">Display Name</span></span>
- <span data-ttu-id="70000-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="70000-152">Is Deleted</span></span>
- <span data-ttu-id="70000-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="70000-153">Deleted Date</span></span>
- <span data-ttu-id="70000-154">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="70000-154">Has Exchange License</span></span>
- <span data-ttu-id="70000-155">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="70000-155">Has OneDrive License</span></span>
- <span data-ttu-id="70000-156">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="70000-156">Has SharePoint License</span></span>
- <span data-ttu-id="70000-157">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="70000-157">Has Skype For Business License</span></span>
- <span data-ttu-id="70000-158">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="70000-158">Has Yammer License</span></span>
- <span data-ttu-id="70000-159">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="70000-159">Has Teams License</span></span>
- <span data-ttu-id="70000-160">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="70000-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="70000-161">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="70000-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="70000-162">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="70000-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="70000-163">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="70000-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="70000-164">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="70000-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="70000-165">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="70000-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="70000-166">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="70000-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="70000-167">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="70000-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="70000-168">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="70000-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="70000-169">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="70000-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="70000-170">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="70000-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="70000-171">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="70000-171">Teams License Assign Date</span></span>
- <span data-ttu-id="70000-172">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="70000-172">Assigned Products</span></span>

<span data-ttu-id="70000-173">Não há suporte para as seguintes colunas na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="70000-173">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="70000-174">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="70000-174">Has Yammer License</span></span>
- <span data-ttu-id="70000-175">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="70000-175">Has Teams License</span></span>
- <span data-ttu-id="70000-176">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="70000-176">Yammer Last Activity Date</span></span>
- <span data-ttu-id="70000-177">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="70000-177">Teams Last Activity Date</span></span>
- <span data-ttu-id="70000-178">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="70000-178">Yammer License Assign Date</span></span>
- <span data-ttu-id="70000-179">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="70000-179">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="70000-180">JSON</span><span class="sxs-lookup"><span data-stu-id="70000-180">JSON</span></span>

<span data-ttu-id="70000-181">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70000-181">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="70000-182">Não há suporte para as seguintes propriedades no objeto **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="70000-182">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="70000-183">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="70000-183">hasYammerLicense</span></span>
- <span data-ttu-id="70000-184">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="70000-184">hasTeamsLicense</span></span>
- <span data-ttu-id="70000-185">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="70000-185">yammerLastActivityDate</span></span>
- <span data-ttu-id="70000-186">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="70000-186">teamsLastActivityDate</span></span>
- <span data-ttu-id="70000-187">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="70000-187">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="70000-188">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="70000-188">teamsLicenseAssignDate</span></span>

<span data-ttu-id="70000-189">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="70000-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="70000-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70000-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="70000-191">CSV</span><span class="sxs-lookup"><span data-stu-id="70000-191">CSV</span></span>

<span data-ttu-id="70000-192">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="70000-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="70000-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70000-193">Request</span></span>

<span data-ttu-id="70000-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70000-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="70000-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="70000-195">Response</span></span>

<span data-ttu-id="70000-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70000-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="70000-197">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="70000-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a><span data-ttu-id="70000-198">JSON</span><span class="sxs-lookup"><span data-stu-id="70000-198">JSON</span></span>

<span data-ttu-id="70000-199">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="70000-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="70000-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70000-200">Request</span></span>

<span data-ttu-id="70000-201">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70000-201">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="70000-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="70000-202">Response</span></span>

<span data-ttu-id="70000-203">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70000-203">The following is an example of the response.</span></span>

> <span data-ttu-id="70000-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70000-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
