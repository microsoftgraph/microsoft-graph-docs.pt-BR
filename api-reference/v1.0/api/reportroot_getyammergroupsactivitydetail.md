# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="fa34c-101">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="fa34c-101">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="fa34c-102">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="fa34c-102">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="fa34c-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="fa34c-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa34c-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa34c-104">Permissions</span></span>

<span data-ttu-id="fa34c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa34c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fa34c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa34c-107">Permission type</span></span>                        | <span data-ttu-id="fa34c-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa34c-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fa34c-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa34c-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa34c-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa34c-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fa34c-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa34c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa34c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa34c-112">Not supported.</span></span>                           |
| <span data-ttu-id="fa34c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa34c-113">Application</span></span>                            | <span data-ttu-id="fa34c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa34c-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fa34c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa34c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="fa34c-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="fa34c-116">Request parameters</span></span>

<span data-ttu-id="fa34c-117">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fa34c-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fa34c-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa34c-118">Parameter</span></span> | <span data-ttu-id="fa34c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa34c-119">Type</span></span>   | <span data-ttu-id="fa34c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa34c-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fa34c-121">ponto</span><span class="sxs-lookup"><span data-stu-id="fa34c-121">period</span></span>    | <span data-ttu-id="fa34c-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa34c-122">string</span></span> | <span data-ttu-id="fa34c-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fa34c-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fa34c-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="fa34c-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fa34c-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fa34c-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fa34c-126">data</span><span class="sxs-lookup"><span data-stu-id="fa34c-126">date</span></span>      | <span data-ttu-id="fa34c-127">Data</span><span class="sxs-lookup"><span data-stu-id="fa34c-127">Date</span></span>   | <span data-ttu-id="fa34c-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="fa34c-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fa34c-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="fa34c-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fa34c-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="fa34c-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fa34c-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="fa34c-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa34c-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa34c-132">Request headers</span></span>

| <span data-ttu-id="fa34c-133">Nome</span><span class="sxs-lookup"><span data-stu-id="fa34c-133">Name</span></span>          | <span data-ttu-id="fa34c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa34c-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fa34c-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa34c-135">Authorization</span></span> | <span data-ttu-id="fa34c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa34c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fa34c-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fa34c-138">If-None-Match</span></span> | <span data-ttu-id="fa34c-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="fa34c-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fa34c-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fa34c-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fa34c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa34c-141">Response</span></span>

<span data-ttu-id="fa34c-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="fa34c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fa34c-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="fa34c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fa34c-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fa34c-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fa34c-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="fa34c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fa34c-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="fa34c-146">Report Refresh Date</span></span>
- <span data-ttu-id="fa34c-147">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="fa34c-147">Group Display Name</span></span>
- <span data-ttu-id="fa34c-148">Excluído</span><span class="sxs-lookup"><span data-stu-id="fa34c-148">Is Deleted</span></span>
- <span data-ttu-id="fa34c-149">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="fa34c-149">Owner Principal Name</span></span>
- <span data-ttu-id="fa34c-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="fa34c-150">Last Activity Date</span></span>
- <span data-ttu-id="fa34c-151">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="fa34c-151">Group Type</span></span>
- <span data-ttu-id="fa34c-152">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="fa34c-152">Office 365 Connected</span></span>
- <span data-ttu-id="fa34c-153">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="fa34c-153">Member Count</span></span>
- <span data-ttu-id="fa34c-154">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="fa34c-154">Posted Count</span></span>
- <span data-ttu-id="fa34c-155">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="fa34c-155">Read Count</span></span>
- <span data-ttu-id="fa34c-156">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="fa34c-156">Liked Count</span></span>
- <span data-ttu-id="fa34c-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="fa34c-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fa34c-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa34c-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fa34c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa34c-159">Request</span></span>

<span data-ttu-id="fa34c-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa34c-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fa34c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa34c-161">Response</span></span>

<span data-ttu-id="fa34c-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa34c-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fa34c-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="fa34c-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
