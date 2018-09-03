# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="e0575-101">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e0575-101">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="e0575-102">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="e0575-102">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="e0575-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="e0575-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0575-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0575-104">Permissions</span></span>

<span data-ttu-id="e0575-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e0575-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0575-107">Permission type</span></span>                        | <span data-ttu-id="e0575-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0575-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e0575-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0575-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0575-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0575-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e0575-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0575-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0575-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0575-112">Not supported.</span></span>                           |
| <span data-ttu-id="e0575-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0575-113">Application</span></span>                            | <span data-ttu-id="e0575-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0575-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e0575-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0575-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e0575-116">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e0575-116">Function parameters</span></span>

<span data-ttu-id="e0575-117">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e0575-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e0575-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e0575-118">Parameter</span></span> | <span data-ttu-id="e0575-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0575-119">Type</span></span>   | <span data-ttu-id="e0575-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0575-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e0575-121">ponto</span><span class="sxs-lookup"><span data-stu-id="e0575-121">period</span></span>    | <span data-ttu-id="e0575-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0575-122">string</span></span> | <span data-ttu-id="e0575-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e0575-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e0575-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e0575-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e0575-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e0575-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e0575-126">data</span><span class="sxs-lookup"><span data-stu-id="e0575-126">date</span></span>      | <span data-ttu-id="e0575-127">Data</span><span class="sxs-lookup"><span data-stu-id="e0575-127">Date</span></span>   | <span data-ttu-id="e0575-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="e0575-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e0575-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="e0575-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e0575-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e0575-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e0575-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="e0575-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0575-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0575-132">Request headers</span></span>

| <span data-ttu-id="e0575-133">Nome</span><span class="sxs-lookup"><span data-stu-id="e0575-133">Name</span></span>          | <span data-ttu-id="e0575-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0575-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e0575-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0575-135">Authorization</span></span> | <span data-ttu-id="e0575-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0575-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e0575-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e0575-138">If-None-Match</span></span> | <span data-ttu-id="e0575-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="e0575-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e0575-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e0575-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e0575-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0575-141">Response</span></span>

<span data-ttu-id="e0575-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e0575-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e0575-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e0575-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e0575-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e0575-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e0575-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e0575-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e0575-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e0575-146">Report Refresh Date</span></span>
- <span data-ttu-id="e0575-147">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="e0575-147">Group Display Name</span></span>
- <span data-ttu-id="e0575-148">Excluído</span><span class="sxs-lookup"><span data-stu-id="e0575-148">Is Deleted</span></span>
- <span data-ttu-id="e0575-149">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="e0575-149">Owner Principal Name</span></span>
- <span data-ttu-id="e0575-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="e0575-150">Last Activity Date</span></span>
- <span data-ttu-id="e0575-151">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="e0575-151">Group Type</span></span>
- <span data-ttu-id="e0575-152">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="e0575-152">Member Count</span></span>
- <span data-ttu-id="e0575-153">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="e0575-153">External Member Count</span></span>
- <span data-ttu-id="e0575-154">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="e0575-154">Exchange Received Email Count</span></span>
- <span data-ttu-id="e0575-155">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="e0575-155">SharePoint Active File Count</span></span>
- <span data-ttu-id="e0575-156">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="e0575-156">Yammer Posted Message Count</span></span>
- <span data-ttu-id="e0575-157">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="e0575-157">Yammer Read Message Count</span></span>
- <span data-ttu-id="e0575-158">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="e0575-158">Yammer Liked Message Count</span></span>
- <span data-ttu-id="e0575-159">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="e0575-159">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="e0575-160">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="e0575-160">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="e0575-161">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="e0575-161">SharePoint Total File Count</span></span>
- <span data-ttu-id="e0575-162">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="e0575-162">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="e0575-163">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e0575-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e0575-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0575-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e0575-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0575-165">Request</span></span>

<span data-ttu-id="e0575-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0575-166">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e0575-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0575-167">Response</span></span>

<span data-ttu-id="e0575-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0575-168">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e0575-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e0575-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```
