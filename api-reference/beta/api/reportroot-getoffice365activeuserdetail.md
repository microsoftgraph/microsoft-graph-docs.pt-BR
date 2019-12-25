---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3192062a7e533995804b0e26bf948277690047e8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869140"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="38a47-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="38a47-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a47-104">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="38a47-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="38a47-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="38a47-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="38a47-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38a47-106">Permissions</span></span>

<span data-ttu-id="38a47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38a47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38a47-109">Permission type</span></span>                        | <span data-ttu-id="38a47-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38a47-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38a47-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38a47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38a47-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38a47-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38a47-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38a47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38a47-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38a47-114">Not supported.</span></span>                           |
| <span data-ttu-id="38a47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38a47-115">Application</span></span>                            | <span data-ttu-id="38a47-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38a47-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="38a47-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="38a47-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="38a47-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="38a47-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="38a47-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38a47-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="38a47-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="38a47-120">Function parameters</span></span>

<span data-ttu-id="38a47-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="38a47-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="38a47-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="38a47-122">Parameter</span></span> | <span data-ttu-id="38a47-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="38a47-123">Type</span></span>   | <span data-ttu-id="38a47-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a47-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38a47-125">ponto</span><span class="sxs-lookup"><span data-stu-id="38a47-125">period</span></span>    | <span data-ttu-id="38a47-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38a47-126">string</span></span> | <span data-ttu-id="38a47-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="38a47-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38a47-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="38a47-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38a47-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="38a47-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="38a47-130">data</span><span class="sxs-lookup"><span data-stu-id="38a47-130">date</span></span>      | <span data-ttu-id="38a47-131">Data</span><span class="sxs-lookup"><span data-stu-id="38a47-131">Date</span></span>   | <span data-ttu-id="38a47-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="38a47-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="38a47-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="38a47-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="38a47-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="38a47-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="38a47-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="38a47-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="38a47-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="38a47-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="38a47-137">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="38a47-137">The default output type is text/csv.</span></span> <span data-ttu-id="38a47-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="38a47-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38a47-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38a47-139">Request headers</span></span>

| <span data-ttu-id="38a47-140">Nome</span><span class="sxs-lookup"><span data-stu-id="38a47-140">Name</span></span>          | <span data-ttu-id="38a47-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a47-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="38a47-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="38a47-142">Authorization</span></span> | <span data-ttu-id="38a47-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38a47-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="38a47-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a47-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="38a47-146">CSV</span><span class="sxs-lookup"><span data-stu-id="38a47-146">CSV</span></span>

<span data-ttu-id="38a47-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="38a47-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38a47-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="38a47-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38a47-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="38a47-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38a47-150">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="38a47-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="38a47-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="38a47-151">Report Refresh Date</span></span>
- <span data-ttu-id="38a47-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="38a47-152">User Principal Name</span></span>
- <span data-ttu-id="38a47-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="38a47-153">Display Name</span></span>
- <span data-ttu-id="38a47-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="38a47-154">Is Deleted</span></span>
- <span data-ttu-id="38a47-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="38a47-155">Deleted Date</span></span>
- <span data-ttu-id="38a47-156">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="38a47-156">Has Exchange License</span></span>
- <span data-ttu-id="38a47-157">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="38a47-157">Has OneDrive License</span></span>
- <span data-ttu-id="38a47-158">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="38a47-158">Has SharePoint License</span></span>
- <span data-ttu-id="38a47-159">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="38a47-159">Has Skype For Business License</span></span>
- <span data-ttu-id="38a47-160">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="38a47-160">Has Yammer License</span></span>
- <span data-ttu-id="38a47-161">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="38a47-161">Has Teams License</span></span>
- <span data-ttu-id="38a47-162">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="38a47-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="38a47-163">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="38a47-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="38a47-164">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="38a47-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="38a47-165">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="38a47-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="38a47-166">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="38a47-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="38a47-167">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="38a47-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="38a47-168">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="38a47-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="38a47-169">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="38a47-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="38a47-170">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="38a47-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="38a47-171">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="38a47-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="38a47-172">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="38a47-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="38a47-173">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="38a47-173">Teams License Assign Date</span></span>
- <span data-ttu-id="38a47-174">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="38a47-174">Assigned Products</span></span>

<span data-ttu-id="38a47-175">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="38a47-175">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="38a47-176">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="38a47-176">Has Yammer License</span></span>
- <span data-ttu-id="38a47-177">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="38a47-177">Has Teams License</span></span>
- <span data-ttu-id="38a47-178">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="38a47-178">Yammer Last Activity Date</span></span>
- <span data-ttu-id="38a47-179">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="38a47-179">Teams Last Activity Date</span></span>
- <span data-ttu-id="38a47-180">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="38a47-180">Yammer License Assign Date</span></span>
- <span data-ttu-id="38a47-181">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="38a47-181">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="38a47-182">JSON</span><span class="sxs-lookup"><span data-stu-id="38a47-182">JSON</span></span>

<span data-ttu-id="38a47-183">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38a47-183">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="38a47-184">As propriedades a seguir no objeto **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="38a47-184">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="38a47-185">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="38a47-185">hasYammerLicense</span></span>
- <span data-ttu-id="38a47-186">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="38a47-186">hasTeamsLicense</span></span>
- <span data-ttu-id="38a47-187">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="38a47-187">yammerLastActivityDate</span></span>
- <span data-ttu-id="38a47-188">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="38a47-188">teamsLastActivityDate</span></span>
- <span data-ttu-id="38a47-189">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="38a47-189">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="38a47-190">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="38a47-190">teamsLicenseAssignDate</span></span>

<span data-ttu-id="38a47-191">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="38a47-191">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="38a47-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38a47-192">Example</span></span>

### <a name="csv"></a><span data-ttu-id="38a47-193">CSV</span><span class="sxs-lookup"><span data-stu-id="38a47-193">CSV</span></span>

<span data-ttu-id="38a47-194">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="38a47-194">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="38a47-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38a47-195">Request</span></span>

<span data-ttu-id="38a47-196">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38a47-196">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="38a47-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="38a47-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38a47-198">C#</span><span class="sxs-lookup"><span data-stu-id="38a47-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38a47-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38a47-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38a47-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38a47-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38a47-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a47-201">Response</span></span>

<span data-ttu-id="38a47-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38a47-202">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="38a47-203">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="38a47-203">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="38a47-204">JSON</span><span class="sxs-lookup"><span data-stu-id="38a47-204">JSON</span></span>

<span data-ttu-id="38a47-205">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="38a47-205">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="38a47-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38a47-206">Request</span></span>

<span data-ttu-id="38a47-207">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38a47-207">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="38a47-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="38a47-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38a47-209">C#</span><span class="sxs-lookup"><span data-stu-id="38a47-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38a47-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38a47-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38a47-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38a47-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38a47-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a47-212">Response</span></span>

<span data-ttu-id="38a47-213">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38a47-213">The following is an example of the response.</span></span>

> <span data-ttu-id="38a47-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38a47-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
