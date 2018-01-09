# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="f6195-101">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f6195-101">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="f6195-102">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="f6195-102">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="f6195-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business]((https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)).</span><span class="sxs-lookup"><span data-stu-id="f6195-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity]((https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6195-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6195-104">Permissions</span></span>

<span data-ttu-id="f6195-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f6195-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6195-107">Permission type</span></span>                        | <span data-ttu-id="f6195-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6195-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f6195-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6195-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6195-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6195-110">Not supported.</span></span>                           |
| <span data-ttu-id="f6195-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6195-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6195-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6195-112">Not supported.</span></span>                           |
| <span data-ttu-id="f6195-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6195-113">Application</span></span>                            | <span data-ttu-id="f6195-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6195-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f6195-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6195-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="f6195-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="f6195-116">Request parameters</span></span>

<span data-ttu-id="f6195-117">Na URL da solicitação, forneça um valor válido ao parâmetro de consulta escolhido.</span><span class="sxs-lookup"><span data-stu-id="f6195-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="f6195-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f6195-118">Parameter</span></span> | <span data-ttu-id="f6195-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6195-119">Type</span></span>   | <span data-ttu-id="f6195-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6195-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f6195-121">ponto</span><span class="sxs-lookup"><span data-stu-id="f6195-121">Period</span></span>    | <span data-ttu-id="f6195-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6195-122">string</span></span> | <span data-ttu-id="f6195-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f6195-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f6195-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f6195-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f6195-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f6195-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f6195-126">data</span><span class="sxs-lookup"><span data-stu-id="f6195-126">date</span></span>      | <span data-ttu-id="f6195-127">Data</span><span class="sxs-lookup"><span data-stu-id="f6195-127">Date</span></span>   | <span data-ttu-id="f6195-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="f6195-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f6195-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f6195-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f6195-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="f6195-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f6195-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="f6195-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6195-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6195-132">Request headers</span></span>

| <span data-ttu-id="f6195-133">Nome</span><span class="sxs-lookup"><span data-stu-id="f6195-133">Name</span></span>          | <span data-ttu-id="f6195-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6195-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f6195-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6195-135">Authorization</span></span> | <span data-ttu-id="f6195-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6195-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f6195-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f6195-138">if-none-match</span></span> | <span data-ttu-id="f6195-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="f6195-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="f6195-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f6195-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f6195-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6195-141">Response</span></span>

<span data-ttu-id="f6195-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f6195-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f6195-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f6195-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f6195-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f6195-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="f6195-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f6195-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f6195-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f6195-146">Report Refresh Date</span></span>
- <span data-ttu-id="f6195-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="f6195-147">User Principal Name</span></span>
- <span data-ttu-id="f6195-148">Excluído</span><span class="sxs-lookup"><span data-stu-id="f6195-148">Is Deleted</span></span>
- <span data-ttu-id="f6195-149">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="f6195-149">Deleted Date</span></span>
- <span data-ttu-id="f6195-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="f6195-150">Last Activity Date</span></span>
- <span data-ttu-id="f6195-151">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="f6195-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="f6195-152">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="f6195-152">Synced File Count</span></span>
- <span data-ttu-id="f6195-153">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="f6195-153">Shared Internally File Count</span></span>
- <span data-ttu-id="f6195-154">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="f6195-154">Shared Externally File Count</span></span>
- <span data-ttu-id="f6195-155">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="f6195-155">Assigned Products</span></span>
- <span data-ttu-id="f6195-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f6195-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f6195-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6195-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f6195-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6195-158">Request</span></span>

<span data-ttu-id="f6195-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6195-159">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f6195-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6195-160">Response</span></span>

<span data-ttu-id="f6195-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6195-161">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f6195-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f6195-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
