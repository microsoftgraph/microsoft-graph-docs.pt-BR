---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obter detalhes sobre a atividade de grupos do Microsoft 365 por grupo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 33e0455d08cd3d853337261a440b5803de419248
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981610"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="2867e-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="2867e-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="2867e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2867e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2867e-105">Obter detalhes sobre a atividade de grupos do Microsoft 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="2867e-105">Get details about Microsoft 365 groups activity by group.</span></span>

> <span data-ttu-id="2867e-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - grupos do Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="2867e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="2867e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2867e-107">Permissions</span></span>

<span data-ttu-id="2867e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2867e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2867e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2867e-110">Permission type</span></span>                        | <span data-ttu-id="2867e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2867e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2867e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2867e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2867e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2867e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2867e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2867e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2867e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2867e-115">Not supported.</span></span>                           |
| <span data-ttu-id="2867e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2867e-116">Application</span></span>                            | <span data-ttu-id="2867e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2867e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="2867e-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="2867e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2867e-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2867e-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2867e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2867e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2867e-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2867e-121">Function parameters</span></span>

<span data-ttu-id="2867e-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2867e-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2867e-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2867e-123">Parameter</span></span> | <span data-ttu-id="2867e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2867e-124">Type</span></span>   | <span data-ttu-id="2867e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2867e-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2867e-126">ponto</span><span class="sxs-lookup"><span data-stu-id="2867e-126">period</span></span>    | <span data-ttu-id="2867e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2867e-127">string</span></span> | <span data-ttu-id="2867e-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2867e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2867e-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="2867e-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2867e-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2867e-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2867e-131">data</span><span class="sxs-lookup"><span data-stu-id="2867e-131">date</span></span>      | <span data-ttu-id="2867e-132">Data</span><span class="sxs-lookup"><span data-stu-id="2867e-132">Date</span></span>   | <span data-ttu-id="2867e-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="2867e-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2867e-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="2867e-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2867e-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="2867e-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2867e-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="2867e-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="2867e-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="2867e-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2867e-138">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="2867e-138">The default output type is text/csv.</span></span> <span data-ttu-id="2867e-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="2867e-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2867e-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2867e-140">Request headers</span></span>

| <span data-ttu-id="2867e-141">Nome</span><span class="sxs-lookup"><span data-stu-id="2867e-141">Name</span></span>          | <span data-ttu-id="2867e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="2867e-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2867e-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="2867e-143">Authorization</span></span> | <span data-ttu-id="2867e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2867e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2867e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2867e-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2867e-147">CSV</span><span class="sxs-lookup"><span data-stu-id="2867e-147">CSV</span></span>

<span data-ttu-id="2867e-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2867e-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2867e-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2867e-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2867e-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2867e-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2867e-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2867e-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2867e-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2867e-152">Report Refresh Date</span></span>
- <span data-ttu-id="2867e-153">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="2867e-153">Group Display Name</span></span>
- <span data-ttu-id="2867e-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="2867e-154">Is Deleted</span></span>
- <span data-ttu-id="2867e-155">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="2867e-155">Owner Principal Name</span></span>
- <span data-ttu-id="2867e-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="2867e-156">Last Activity Date</span></span>
- <span data-ttu-id="2867e-157">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="2867e-157">Group Type</span></span>
- <span data-ttu-id="2867e-158">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="2867e-158">Member Count</span></span>
- <span data-ttu-id="2867e-159">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="2867e-159">External Member Count</span></span>
- <span data-ttu-id="2867e-160">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="2867e-160">Exchange Received Email Count</span></span>
- <span data-ttu-id="2867e-161">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="2867e-161">SharePoint Active File Count</span></span>
- <span data-ttu-id="2867e-162">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="2867e-162">Yammer Posted Message Count</span></span>
- <span data-ttu-id="2867e-163">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="2867e-163">Yammer Read Message Count</span></span>
- <span data-ttu-id="2867e-164">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="2867e-164">Yammer Liked Message Count</span></span>
- <span data-ttu-id="2867e-165">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="2867e-165">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="2867e-166">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="2867e-166">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="2867e-167">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="2867e-167">SharePoint Total File Count</span></span>
- <span data-ttu-id="2867e-168">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="2867e-168">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="2867e-169">ID do Grupo</span><span class="sxs-lookup"><span data-stu-id="2867e-169">Group Id</span></span>
- <span data-ttu-id="2867e-170">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="2867e-170">Report Period</span></span>

<span data-ttu-id="2867e-171">As seguintes colunas não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="2867e-171">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="2867e-172">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="2867e-172">Yammer Posted Message Count</span></span>
- <span data-ttu-id="2867e-173">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="2867e-173">Yammer Read Message Count</span></span>
- <span data-ttu-id="2867e-174">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="2867e-174">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="2867e-175">JSON</span><span class="sxs-lookup"><span data-stu-id="2867e-175">JSON</span></span>

<span data-ttu-id="2867e-176">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2867e-176">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="2867e-177">As seguintes propriedades no **[objeto office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="2867e-177">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="2867e-178">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="2867e-178">yammerPostedMessageCount</span></span>
- <span data-ttu-id="2867e-179">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="2867e-179">yammerReadMessageCount</span></span>
- <span data-ttu-id="2867e-180">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="2867e-180">yammerLikedMessageCount</span></span>

<span data-ttu-id="2867e-181">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="2867e-181">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="2867e-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2867e-182">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2867e-183">CSV</span><span class="sxs-lookup"><span data-stu-id="2867e-183">CSV</span></span>

<span data-ttu-id="2867e-184">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="2867e-184">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2867e-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2867e-185">Request</span></span>

<span data-ttu-id="2867e-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2867e-186">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="2867e-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="2867e-187">Response</span></span>

<span data-ttu-id="2867e-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2867e-188">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2867e-189">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2867e-189">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
```

### <a name="json"></a><span data-ttu-id="2867e-190">JSON</span><span class="sxs-lookup"><span data-stu-id="2867e-190">JSON</span></span>

<span data-ttu-id="2867e-191">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="2867e-191">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2867e-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2867e-192">Request</span></span>

<span data-ttu-id="2867e-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2867e-193">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="2867e-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="2867e-194">Response</span></span>

<span data-ttu-id="2867e-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2867e-195">The following is an example of the response.</span></span>

> <span data-ttu-id="2867e-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2867e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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


