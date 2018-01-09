# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="cd82d-101">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="cd82d-101">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="cd82d-102">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cd82d-102">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="cd82d-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint]((https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)).</span><span class="sxs-lookup"><span data-stu-id="cd82d-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage]((https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd82d-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd82d-104">Permissions</span></span>

<span data-ttu-id="cd82d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd82d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cd82d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd82d-107">Permission type</span></span>                        | <span data-ttu-id="cd82d-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd82d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cd82d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd82d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd82d-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd82d-110">Not supported.</span></span>                           |
| <span data-ttu-id="cd82d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd82d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd82d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd82d-112">Not supported.</span></span>                           |
| <span data-ttu-id="cd82d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd82d-113">Application</span></span>                            | <span data-ttu-id="cd82d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd82d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cd82d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd82d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="cd82d-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="cd82d-116">Request parameters</span></span>

<span data-ttu-id="cd82d-117">Na URL da solicitação, forneça um valor válido ao parâmetro de consulta escolhido.</span><span class="sxs-lookup"><span data-stu-id="cd82d-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="cd82d-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cd82d-118">Parameter</span></span> | <span data-ttu-id="cd82d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd82d-119">Type</span></span>   | <span data-ttu-id="cd82d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd82d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cd82d-121">ponto</span><span class="sxs-lookup"><span data-stu-id="cd82d-121">Period</span></span>    | <span data-ttu-id="cd82d-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd82d-122">string</span></span> | <span data-ttu-id="cd82d-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cd82d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cd82d-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="cd82d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cd82d-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cd82d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="cd82d-126">data</span><span class="sxs-lookup"><span data-stu-id="cd82d-126">date</span></span>      | <span data-ttu-id="cd82d-127">Data</span><span class="sxs-lookup"><span data-stu-id="cd82d-127">Date</span></span>   | <span data-ttu-id="cd82d-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="cd82d-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="cd82d-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="cd82d-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="cd82d-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="cd82d-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="cd82d-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="cd82d-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd82d-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd82d-132">Request headers</span></span>

| <span data-ttu-id="cd82d-133">Nome</span><span class="sxs-lookup"><span data-stu-id="cd82d-133">Name</span></span>          | <span data-ttu-id="cd82d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd82d-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cd82d-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd82d-135">Authorization</span></span> | <span data-ttu-id="cd82d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd82d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd82d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cd82d-138">if-none-match</span></span> | <span data-ttu-id="cd82d-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="cd82d-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="cd82d-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cd82d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cd82d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd82d-141">Response</span></span>

<span data-ttu-id="cd82d-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="cd82d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cd82d-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="cd82d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cd82d-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cd82d-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="cd82d-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="cd82d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cd82d-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="cd82d-146">Report Refresh Date</span></span>
- <span data-ttu-id="cd82d-147">URL do site</span><span class="sxs-lookup"><span data-stu-id="cd82d-147">Site URL</span></span>
- <span data-ttu-id="cd82d-148">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="cd82d-148">Owner Display Name</span></span>
- <span data-ttu-id="cd82d-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="cd82d-149">Is Deleted</span></span>
- <span data-ttu-id="cd82d-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="cd82d-150">Last Activity Date</span></span>
- <span data-ttu-id="cd82d-151">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="cd82d-151">File Count</span></span>
- <span data-ttu-id="cd82d-152">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="cd82d-152">Active File Count</span></span>
- <span data-ttu-id="cd82d-153">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="cd82d-153">Page View Count</span></span>
- <span data-ttu-id="cd82d-154">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="cd82d-154">Visited Page Count</span></span>
- <span data-ttu-id="cd82d-155">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="cd82d-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="cd82d-156">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="cd82d-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="cd82d-157">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="cd82d-157">Root Web Template</span></span>
- <span data-ttu-id="cd82d-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="cd82d-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cd82d-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd82d-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cd82d-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd82d-160">Request</span></span>

<span data-ttu-id="cd82d-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd82d-161">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="cd82d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd82d-162">Response</span></span>

<span data-ttu-id="cd82d-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd82d-163">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cd82d-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="cd82d-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```
