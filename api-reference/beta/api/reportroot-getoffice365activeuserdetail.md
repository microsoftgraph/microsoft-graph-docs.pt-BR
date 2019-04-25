---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 55549d2872232f292eeaabff550b1612ad2d1657
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538235"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="474b4-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="474b4-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="474b4-104">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="474b4-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="474b4-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="474b4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="474b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="474b4-106">Permissions</span></span>

<span data-ttu-id="474b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="474b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="474b4-109">Permission type</span></span>                        | <span data-ttu-id="474b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="474b4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="474b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="474b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="474b4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="474b4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="474b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="474b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="474b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="474b4-114">Not supported.</span></span>                           |
| <span data-ttu-id="474b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="474b4-115">Application</span></span>                            | <span data-ttu-id="474b4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="474b4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="474b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="474b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="474b4-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="474b4-118">Function parameters</span></span>

<span data-ttu-id="474b4-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="474b4-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="474b4-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="474b4-120">Parameter</span></span> | <span data-ttu-id="474b4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="474b4-121">Type</span></span>   | <span data-ttu-id="474b4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="474b4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="474b4-123">ponto</span><span class="sxs-lookup"><span data-stu-id="474b4-123">period</span></span>    | <span data-ttu-id="474b4-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="474b4-124">string</span></span> | <span data-ttu-id="474b4-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="474b4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="474b4-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="474b4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="474b4-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="474b4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="474b4-128">data</span><span class="sxs-lookup"><span data-stu-id="474b4-128">date</span></span>      | <span data-ttu-id="474b4-129">Data</span><span class="sxs-lookup"><span data-stu-id="474b4-129">Date</span></span>   | <span data-ttu-id="474b4-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="474b4-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="474b4-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="474b4-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="474b4-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="474b4-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="474b4-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="474b4-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="474b4-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="474b4-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="474b4-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="474b4-135">The default output type is text/csv.</span></span> <span data-ttu-id="474b4-136">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="474b4-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="474b4-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="474b4-137">Request headers</span></span>

| <span data-ttu-id="474b4-138">Nome</span><span class="sxs-lookup"><span data-stu-id="474b4-138">Name</span></span>          | <span data-ttu-id="474b4-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="474b4-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="474b4-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="474b4-140">Authorization</span></span> | <span data-ttu-id="474b4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="474b4-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="474b4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="474b4-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="474b4-144">CSV</span><span class="sxs-lookup"><span data-stu-id="474b4-144">CSV</span></span>

<span data-ttu-id="474b4-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="474b4-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="474b4-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="474b4-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="474b4-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="474b4-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="474b4-148">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="474b4-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="474b4-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="474b4-149">Report Refresh Date</span></span>
- <span data-ttu-id="474b4-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="474b4-150">User Principal Name</span></span>
- <span data-ttu-id="474b4-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="474b4-151">Display Name</span></span>
- <span data-ttu-id="474b4-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="474b4-152">Is Deleted</span></span>
- <span data-ttu-id="474b4-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="474b4-153">Deleted Date</span></span>
- <span data-ttu-id="474b4-154">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="474b4-154">Has Exchange License</span></span>
- <span data-ttu-id="474b4-155">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="474b4-155">Has OneDrive License</span></span>
- <span data-ttu-id="474b4-156">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="474b4-156">Has SharePoint License</span></span>
- <span data-ttu-id="474b4-157">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="474b4-157">Has Skype For Business License</span></span>
- <span data-ttu-id="474b4-158">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="474b4-158">Has Yammer License</span></span>
- <span data-ttu-id="474b4-159">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="474b4-159">Has Teams License</span></span>
- <span data-ttu-id="474b4-160">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="474b4-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="474b4-161">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="474b4-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="474b4-162">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="474b4-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="474b4-163">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="474b4-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="474b4-164">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="474b4-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="474b4-165">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="474b4-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="474b4-166">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="474b4-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="474b4-167">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="474b4-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="474b4-168">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="474b4-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="474b4-169">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="474b4-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="474b4-170">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="474b4-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="474b4-171">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="474b4-171">Teams License Assign Date</span></span>
- <span data-ttu-id="474b4-172">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="474b4-172">Assigned Products</span></span>

<span data-ttu-id="474b4-173">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="474b4-173">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="474b4-174">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="474b4-174">Has Yammer License</span></span>
- <span data-ttu-id="474b4-175">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="474b4-175">Has Teams License</span></span>
- <span data-ttu-id="474b4-176">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="474b4-176">Yammer Last Activity Date</span></span>
- <span data-ttu-id="474b4-177">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="474b4-177">Teams Last Activity Date</span></span>
- <span data-ttu-id="474b4-178">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="474b4-178">Yammer License Assign Date</span></span>
- <span data-ttu-id="474b4-179">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="474b4-179">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="474b4-180">JSON</span><span class="sxs-lookup"><span data-stu-id="474b4-180">JSON</span></span>

<span data-ttu-id="474b4-181">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="474b4-181">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="474b4-182">As propriedades a seguir no objeto **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="474b4-182">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="474b4-183">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="474b4-183">hasYammerLicense</span></span>
- <span data-ttu-id="474b4-184">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="474b4-184">hasTeamsLicense</span></span>
- <span data-ttu-id="474b4-185">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="474b4-185">yammerLastActivityDate</span></span>
- <span data-ttu-id="474b4-186">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="474b4-186">teamsLastActivityDate</span></span>
- <span data-ttu-id="474b4-187">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="474b4-187">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="474b4-188">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="474b4-188">teamsLicenseAssignDate</span></span>

<span data-ttu-id="474b4-189">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="474b4-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="474b4-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="474b4-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="474b4-191">CSV</span><span class="sxs-lookup"><span data-stu-id="474b4-191">CSV</span></span>

<span data-ttu-id="474b4-192">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="474b4-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="474b4-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="474b4-193">Request</span></span>

<span data-ttu-id="474b4-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="474b4-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="474b4-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="474b4-195">Response</span></span>

<span data-ttu-id="474b4-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="474b4-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="474b4-197">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="474b4-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="474b4-198">JSON</span><span class="sxs-lookup"><span data-stu-id="474b4-198">JSON</span></span>

<span data-ttu-id="474b4-199">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="474b4-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="474b4-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="474b4-200">Request</span></span>

<span data-ttu-id="474b4-201">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="474b4-201">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="474b4-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="474b4-202">Response</span></span>

<span data-ttu-id="474b4-203">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="474b4-203">The following is an example of the response.</span></span>

> <span data-ttu-id="474b4-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="474b4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
