---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b7725ca7f56db7873d49729518a37dd3934ed3d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446882"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="6dff3-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="6dff3-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dff3-104">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="6dff3-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="6dff3-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="6dff3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="6dff3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dff3-106">Permissions</span></span>

<span data-ttu-id="6dff3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dff3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dff3-109">Permission type</span></span>                        | <span data-ttu-id="6dff3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dff3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6dff3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dff3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dff3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dff3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6dff3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dff3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dff3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dff3-114">Not supported.</span></span>                           |
| <span data-ttu-id="6dff3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dff3-115">Application</span></span>                            | <span data-ttu-id="6dff3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dff3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6dff3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dff3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6dff3-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6dff3-118">Function parameters</span></span>

<span data-ttu-id="6dff3-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6dff3-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6dff3-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6dff3-120">Parameter</span></span> | <span data-ttu-id="6dff3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dff3-121">Type</span></span>   | <span data-ttu-id="6dff3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dff3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6dff3-123">ponto</span><span class="sxs-lookup"><span data-stu-id="6dff3-123">period</span></span>    | <span data-ttu-id="6dff3-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dff3-124">string</span></span> | <span data-ttu-id="6dff3-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6dff3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6dff3-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6dff3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6dff3-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6dff3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6dff3-128">data</span><span class="sxs-lookup"><span data-stu-id="6dff3-128">date</span></span>      | <span data-ttu-id="6dff3-129">Data</span><span class="sxs-lookup"><span data-stu-id="6dff3-129">Date</span></span>   | <span data-ttu-id="6dff3-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="6dff3-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6dff3-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="6dff3-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6dff3-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="6dff3-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6dff3-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="6dff3-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="6dff3-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff3-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6dff3-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="6dff3-135">The default output type is text/csv.</span></span> <span data-ttu-id="6dff3-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6dff3-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dff3-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dff3-137">Request headers</span></span>

| <span data-ttu-id="6dff3-138">Nome</span><span class="sxs-lookup"><span data-stu-id="6dff3-138">Name</span></span>          | <span data-ttu-id="6dff3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dff3-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6dff3-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dff3-140">Authorization</span></span> | <span data-ttu-id="6dff3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dff3-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6dff3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dff3-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6dff3-144">CSV</span><span class="sxs-lookup"><span data-stu-id="6dff3-144">CSV</span></span>

<span data-ttu-id="6dff3-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6dff3-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6dff3-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff3-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6dff3-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6dff3-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6dff3-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6dff3-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6dff3-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6dff3-149">Report Refresh Date</span></span>
- <span data-ttu-id="6dff3-150">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="6dff3-150">Group Display Name</span></span>
- <span data-ttu-id="6dff3-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="6dff3-151">Is Deleted</span></span>
- <span data-ttu-id="6dff3-152">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="6dff3-152">Owner Principal Name</span></span>
- <span data-ttu-id="6dff3-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="6dff3-153">Last Activity Date</span></span>
- <span data-ttu-id="6dff3-154">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="6dff3-154">Group Type</span></span>
- <span data-ttu-id="6dff3-155">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="6dff3-155">Member Count</span></span>
- <span data-ttu-id="6dff3-156">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="6dff3-156">External Member Count</span></span>
- <span data-ttu-id="6dff3-157">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="6dff3-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="6dff3-158">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="6dff3-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="6dff3-159">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="6dff3-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="6dff3-160">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="6dff3-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="6dff3-161">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="6dff3-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="6dff3-162">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="6dff3-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="6dff3-163">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="6dff3-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="6dff3-164">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="6dff3-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="6dff3-165">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="6dff3-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="6dff3-166">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6dff3-166">Report Period</span></span>

<span data-ttu-id="6dff3-167">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="6dff3-167">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6dff3-168">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="6dff3-168">Yammer Posted Message Count</span></span>
- <span data-ttu-id="6dff3-169">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="6dff3-169">Yammer Read Message Count</span></span>
- <span data-ttu-id="6dff3-170">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="6dff3-170">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="6dff3-171">JSON</span><span class="sxs-lookup"><span data-stu-id="6dff3-171">JSON</span></span>

<span data-ttu-id="6dff3-172">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff3-172">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="6dff3-173">As propriedades a seguir no objeto **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="6dff3-173">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6dff3-174">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="6dff3-174">yammerPostedMessageCount</span></span>
- <span data-ttu-id="6dff3-175">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="6dff3-175">yammerReadMessageCount</span></span>
- <span data-ttu-id="6dff3-176">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="6dff3-176">yammerLikedMessageCount</span></span>

<span data-ttu-id="6dff3-177">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="6dff3-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="6dff3-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dff3-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6dff3-179">CSV</span><span class="sxs-lookup"><span data-stu-id="6dff3-179">CSV</span></span>

<span data-ttu-id="6dff3-180">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="6dff3-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6dff3-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dff3-181">Request</span></span>

<span data-ttu-id="6dff3-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dff3-182">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6dff3-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dff3-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dff3-184">C#</span><span class="sxs-lookup"><span data-stu-id="6dff3-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dff3-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="6dff3-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dff3-186">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6dff3-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6dff3-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dff3-187">Response</span></span>

<span data-ttu-id="6dff3-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff3-188">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6dff3-189">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6dff3-189">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="6dff3-190">JSON</span><span class="sxs-lookup"><span data-stu-id="6dff3-190">JSON</span></span>

<span data-ttu-id="6dff3-191">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="6dff3-191">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6dff3-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dff3-192">Request</span></span>

<span data-ttu-id="6dff3-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dff3-193">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6dff3-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dff3-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dff3-195">C#</span><span class="sxs-lookup"><span data-stu-id="6dff3-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dff3-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="6dff3-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dff3-197">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6dff3-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6dff3-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dff3-198">Response</span></span>

<span data-ttu-id="6dff3-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff3-199">The following is an example of the response.</span></span>

> <span data-ttu-id="6dff3-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dff3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerDisplayName-value", 
      "lastActivityDate": "2017-08-31", 
      "groupType": "Private", 
      "memberCount": 5, 
      "externalMemberCount": 0, 
      "exchangeReceivedEmailCount": 341, 
      "sharePointActiveFileCount": 0, 
      "yammerPostedMessageCount": 0, 
      "yammerReadMessageCount": 0, 
      "yammerLikedMessageCount": 0, 
      "exchangeMailboxTotalItemCount": 343, 
      "exchangeMailboxStorageUsedInBytes": 3724609, 
      "sharePointTotalFileCount": 0, 
      "sharePointSiteStorageUsedInBytes": 0, 
      "reportPeriod": "30"
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
