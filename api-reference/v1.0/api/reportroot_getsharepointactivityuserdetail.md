# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="8cc42-101">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8cc42-101">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="8cc42-102">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="8cc42-102">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="8cc42-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="8cc42-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc42-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc42-104">Permissions</span></span>

<span data-ttu-id="8cc42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8cc42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8cc42-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc42-107">Permission type</span></span>                        | <span data-ttu-id="8cc42-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc42-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8cc42-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc42-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cc42-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cc42-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8cc42-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc42-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc42-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc42-112">Not supported.</span></span>                           |
| <span data-ttu-id="8cc42-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc42-113">Application</span></span>                            | <span data-ttu-id="8cc42-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cc42-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8cc42-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc42-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="8cc42-116">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8cc42-116">Function parameters</span></span>

<span data-ttu-id="8cc42-117">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8cc42-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8cc42-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8cc42-118">Parameter</span></span> | <span data-ttu-id="8cc42-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc42-119">Type</span></span>   | <span data-ttu-id="8cc42-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc42-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8cc42-121">ponto</span><span class="sxs-lookup"><span data-stu-id="8cc42-121">period</span></span>    | <span data-ttu-id="8cc42-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc42-122">string</span></span> | <span data-ttu-id="8cc42-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8cc42-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8cc42-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8cc42-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8cc42-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8cc42-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8cc42-126">data</span><span class="sxs-lookup"><span data-stu-id="8cc42-126">date</span></span>      | <span data-ttu-id="8cc42-127">Data</span><span class="sxs-lookup"><span data-stu-id="8cc42-127">Date</span></span>   | <span data-ttu-id="8cc42-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="8cc42-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8cc42-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="8cc42-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8cc42-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="8cc42-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8cc42-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="8cc42-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cc42-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc42-132">Request headers</span></span>

| <span data-ttu-id="8cc42-133">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc42-133">Name</span></span>          | <span data-ttu-id="8cc42-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc42-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8cc42-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc42-135">Authorization</span></span> | <span data-ttu-id="8cc42-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc42-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8cc42-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8cc42-138">If-None-Match</span></span> | <span data-ttu-id="8cc42-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="8cc42-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8cc42-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8cc42-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8cc42-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc42-141">Response</span></span>

<span data-ttu-id="8cc42-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8cc42-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8cc42-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc42-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8cc42-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8cc42-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8cc42-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8cc42-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8cc42-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8cc42-146">Report Refresh Date</span></span>
- <span data-ttu-id="8cc42-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="8cc42-147">User Principal Name</span></span>
- <span data-ttu-id="8cc42-148">Excluído</span><span class="sxs-lookup"><span data-stu-id="8cc42-148">Is Deleted</span></span>
- <span data-ttu-id="8cc42-149">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="8cc42-149">Deleted Date</span></span>
- <span data-ttu-id="8cc42-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="8cc42-150">Last Activity Date</span></span>
- <span data-ttu-id="8cc42-151">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="8cc42-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="8cc42-152">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="8cc42-152">Synced File Count</span></span>
- <span data-ttu-id="8cc42-153">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="8cc42-153">Shared Internally File Count</span></span>
- <span data-ttu-id="8cc42-154">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="8cc42-154">Shared Externally File Count</span></span>
- <span data-ttu-id="8cc42-155">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="8cc42-155">Visited Page Count</span></span>
- <span data-ttu-id="8cc42-156">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="8cc42-156">Assigned Products</span></span>
- <span data-ttu-id="8cc42-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8cc42-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8cc42-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc42-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8cc42-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc42-159">Request</span></span>

<span data-ttu-id="8cc42-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc42-160">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8cc42-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc42-161">Response</span></span>

<span data-ttu-id="8cc42-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc42-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="8cc42-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8cc42-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```
