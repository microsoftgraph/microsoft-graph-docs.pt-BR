# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="76ac2-101">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="76ac2-101">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="76ac2-102">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="76ac2-102">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="76ac2-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="76ac2-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="76ac2-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="76ac2-104">Permissions</span></span>

<span data-ttu-id="76ac2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="76ac2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76ac2-107">Permission type</span></span>                        | <span data-ttu-id="76ac2-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76ac2-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="76ac2-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76ac2-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="76ac2-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76ac2-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="76ac2-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76ac2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76ac2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76ac2-112">Not supported.</span></span>                           |
| <span data-ttu-id="76ac2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76ac2-113">Application</span></span>                            | <span data-ttu-id="76ac2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76ac2-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="76ac2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76ac2-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="76ac2-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="76ac2-116">Request parameters</span></span>

<span data-ttu-id="76ac2-117">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="76ac2-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="76ac2-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76ac2-118">Parameter</span></span> | <span data-ttu-id="76ac2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="76ac2-119">Type</span></span>   | <span data-ttu-id="76ac2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="76ac2-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="76ac2-121">ponto</span><span class="sxs-lookup"><span data-stu-id="76ac2-121">period</span></span>    | <span data-ttu-id="76ac2-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76ac2-122">string</span></span> | <span data-ttu-id="76ac2-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="76ac2-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="76ac2-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="76ac2-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="76ac2-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="76ac2-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="76ac2-126">data</span><span class="sxs-lookup"><span data-stu-id="76ac2-126">date</span></span>      | <span data-ttu-id="76ac2-127">Data</span><span class="sxs-lookup"><span data-stu-id="76ac2-127">Date</span></span>   | <span data-ttu-id="76ac2-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="76ac2-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="76ac2-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="76ac2-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="76ac2-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="76ac2-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="76ac2-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="76ac2-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76ac2-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76ac2-132">Request headers</span></span>

| <span data-ttu-id="76ac2-133">Nome</span><span class="sxs-lookup"><span data-stu-id="76ac2-133">Name</span></span>          | <span data-ttu-id="76ac2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="76ac2-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="76ac2-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="76ac2-135">Authorization</span></span> | <span data-ttu-id="76ac2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76ac2-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="76ac2-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="76ac2-138">If-None-Match</span></span> | <span data-ttu-id="76ac2-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="76ac2-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="76ac2-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="76ac2-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="76ac2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="76ac2-141">Response</span></span>

<span data-ttu-id="76ac2-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="76ac2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="76ac2-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="76ac2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="76ac2-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="76ac2-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="76ac2-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="76ac2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="76ac2-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="76ac2-146">Report Refresh Date</span></span>
- <span data-ttu-id="76ac2-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="76ac2-147">User Principal Name</span></span>
- <span data-ttu-id="76ac2-148">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="76ac2-148">Display Name</span></span>
- <span data-ttu-id="76ac2-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="76ac2-149">Is Deleted</span></span>
- <span data-ttu-id="76ac2-150">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="76ac2-150">Deleted Date</span></span>
- <span data-ttu-id="76ac2-151">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="76ac2-151">Last Activity Date</span></span>
- <span data-ttu-id="76ac2-152">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="76ac2-152">Mail For Mac</span></span>
- <span data-ttu-id="76ac2-153">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="76ac2-153">Outlook For Mac</span></span>
- <span data-ttu-id="76ac2-154">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="76ac2-154">Outlook For Windows</span></span>
- <span data-ttu-id="76ac2-155">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="76ac2-155">Outlook For Mobile</span></span>
- <span data-ttu-id="76ac2-156">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="76ac2-156">Other For Mobile</span></span>
- <span data-ttu-id="76ac2-157">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="76ac2-157">Outlook For Web</span></span>
- <span data-ttu-id="76ac2-158">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="76ac2-158">POP3 App</span></span>
- <span data-ttu-id="76ac2-159">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="76ac2-159">IMAP4 App</span></span>
- <span data-ttu-id="76ac2-160">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="76ac2-160">SMTP App</span></span>
- <span data-ttu-id="76ac2-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="76ac2-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="76ac2-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76ac2-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="76ac2-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76ac2-163">Request</span></span>

<span data-ttu-id="76ac2-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76ac2-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="76ac2-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="76ac2-165">Response</span></span>

<span data-ttu-id="76ac2-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76ac2-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="76ac2-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="76ac2-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
