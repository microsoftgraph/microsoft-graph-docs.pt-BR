---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obter detalhes sobre usuários ativos do Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 1d3dab6008e54a464c6b8a62cd90b0b9fed9388e
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983101"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="35337-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="35337-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="35337-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35337-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35337-105">Obter detalhes sobre usuários ativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="35337-105">Get details about Microsoft 365 active users.</span></span>

> <span data-ttu-id="35337-106">**Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Usuários Ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d). </span><span class="sxs-lookup"><span data-stu-id="35337-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="35337-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="35337-107">Permissions</span></span>

<span data-ttu-id="35337-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35337-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35337-110">Permission type</span></span>                        | <span data-ttu-id="35337-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35337-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="35337-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35337-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="35337-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35337-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="35337-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35337-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35337-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35337-115">Not supported.</span></span>                           |
| <span data-ttu-id="35337-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35337-116">Application</span></span>                            | <span data-ttu-id="35337-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35337-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="35337-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="35337-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="35337-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="35337-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="35337-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35337-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="35337-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="35337-121">Function parameters</span></span>

<span data-ttu-id="35337-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="35337-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="35337-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="35337-123">Parameter</span></span> | <span data-ttu-id="35337-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="35337-124">Type</span></span>   | <span data-ttu-id="35337-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="35337-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="35337-126">ponto</span><span class="sxs-lookup"><span data-stu-id="35337-126">period</span></span>    | <span data-ttu-id="35337-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35337-127">string</span></span> | <span data-ttu-id="35337-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="35337-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="35337-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="35337-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="35337-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="35337-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="35337-131">data</span><span class="sxs-lookup"><span data-stu-id="35337-131">date</span></span>      | <span data-ttu-id="35337-132">Data</span><span class="sxs-lookup"><span data-stu-id="35337-132">Date</span></span>   | <span data-ttu-id="35337-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="35337-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="35337-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="35337-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="35337-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="35337-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="35337-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="35337-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="35337-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="35337-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="35337-138">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="35337-138">The default output type is text/csv.</span></span> <span data-ttu-id="35337-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="35337-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35337-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35337-140">Request headers</span></span>

| <span data-ttu-id="35337-141">Nome</span><span class="sxs-lookup"><span data-stu-id="35337-141">Name</span></span>          | <span data-ttu-id="35337-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="35337-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="35337-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="35337-143">Authorization</span></span> | <span data-ttu-id="35337-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35337-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="35337-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="35337-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="35337-147">CSV</span><span class="sxs-lookup"><span data-stu-id="35337-147">CSV</span></span>

<span data-ttu-id="35337-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="35337-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="35337-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="35337-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="35337-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="35337-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="35337-151">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="35337-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="35337-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="35337-152">Report Refresh Date</span></span>
- <span data-ttu-id="35337-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="35337-153">User Principal Name</span></span>
- <span data-ttu-id="35337-154">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="35337-154">Display Name</span></span>
- <span data-ttu-id="35337-155">Excluído</span><span class="sxs-lookup"><span data-stu-id="35337-155">Is Deleted</span></span>
- <span data-ttu-id="35337-156">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="35337-156">Deleted Date</span></span>
- <span data-ttu-id="35337-157">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="35337-157">Has Exchange License</span></span>
- <span data-ttu-id="35337-158">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="35337-158">Has OneDrive License</span></span>
- <span data-ttu-id="35337-159">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="35337-159">Has SharePoint License</span></span>
- <span data-ttu-id="35337-160">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="35337-160">Has Skype For Business License</span></span>
- <span data-ttu-id="35337-161">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="35337-161">Has Yammer License</span></span>
- <span data-ttu-id="35337-162">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="35337-162">Has Teams License</span></span>
- <span data-ttu-id="35337-163">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="35337-163">Exchange Last Activity Date</span></span>
- <span data-ttu-id="35337-164">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="35337-164">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="35337-165">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="35337-165">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="35337-166">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="35337-166">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="35337-167">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="35337-167">Yammer Last Activity Date</span></span>
- <span data-ttu-id="35337-168">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="35337-168">Teams Last Activity Date</span></span>
- <span data-ttu-id="35337-169">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="35337-169">Exchange License Assign Date</span></span>
- <span data-ttu-id="35337-170">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="35337-170">OneDrive License Assign Date</span></span>
- <span data-ttu-id="35337-171">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="35337-171">SharePoint License Assign Date</span></span>
- <span data-ttu-id="35337-172">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="35337-172">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="35337-173">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="35337-173">Yammer License Assign Date</span></span>
- <span data-ttu-id="35337-174">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="35337-174">Teams License Assign Date</span></span>
- <span data-ttu-id="35337-175">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="35337-175">Assigned Products</span></span>

<span data-ttu-id="35337-176">As seguintes colunas não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="35337-176">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="35337-177">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="35337-177">Has Yammer License</span></span>
- <span data-ttu-id="35337-178">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="35337-178">Has Teams License</span></span>
- <span data-ttu-id="35337-179">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="35337-179">Yammer Last Activity Date</span></span>
- <span data-ttu-id="35337-180">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="35337-180">Teams Last Activity Date</span></span>
- <span data-ttu-id="35337-181">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="35337-181">Yammer License Assign Date</span></span>
- <span data-ttu-id="35337-182">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="35337-182">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="35337-183">JSON</span><span class="sxs-lookup"><span data-stu-id="35337-183">JSON</span></span>

<span data-ttu-id="35337-184">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35337-184">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="35337-185">As seguintes propriedades no **[objeto office365ActiveUserDetail](../resources/office365activeuserdetail.md)** não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="35337-185">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="35337-186">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="35337-186">hasYammerLicense</span></span>
- <span data-ttu-id="35337-187">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="35337-187">hasTeamsLicense</span></span>
- <span data-ttu-id="35337-188">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="35337-188">yammerLastActivityDate</span></span>
- <span data-ttu-id="35337-189">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="35337-189">teamsLastActivityDate</span></span>
- <span data-ttu-id="35337-190">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="35337-190">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="35337-191">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="35337-191">teamsLicenseAssignDate</span></span>

<span data-ttu-id="35337-192">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="35337-192">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="35337-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35337-193">Example</span></span>

### <a name="csv"></a><span data-ttu-id="35337-194">CSV</span><span class="sxs-lookup"><span data-stu-id="35337-194">CSV</span></span>

<span data-ttu-id="35337-195">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="35337-195">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="35337-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35337-196">Request</span></span>

<span data-ttu-id="35337-197">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35337-197">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="35337-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="35337-198">Response</span></span>

<span data-ttu-id="35337-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35337-199">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="35337-200">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="35337-200">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="35337-201">JSON</span><span class="sxs-lookup"><span data-stu-id="35337-201">JSON</span></span>

<span data-ttu-id="35337-202">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="35337-202">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="35337-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35337-203">Request</span></span>

<span data-ttu-id="35337-204">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35337-204">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="35337-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="35337-205">Response</span></span>

<span data-ttu-id="35337-206">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35337-206">The following is an example of the response.</span></span>

> <span data-ttu-id="35337-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35337-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "Microsoft 365 ENTERPRISE E5"
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


