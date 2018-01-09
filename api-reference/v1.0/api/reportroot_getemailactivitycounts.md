# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="fafff-101">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="fafff-101">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="fafff-102">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="fafff-102">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="fafff-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email]((https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)).</span><span class="sxs-lookup"><span data-stu-id="fafff-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity]((https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)).</span></span>

## <a name="permissions"></a><span data-ttu-id="fafff-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="fafff-104">Permissions</span></span>

<span data-ttu-id="fafff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fafff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fafff-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fafff-107">Permission type</span></span>                        | <span data-ttu-id="fafff-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fafff-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fafff-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fafff-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fafff-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fafff-110">Not supported.</span></span>                           |
| <span data-ttu-id="fafff-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fafff-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fafff-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fafff-112">Not supported.</span></span>                           |
| <span data-ttu-id="fafff-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fafff-113">Application</span></span>                            | <span data-ttu-id="fafff-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fafff-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fafff-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fafff-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="fafff-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="fafff-116">Request parameters</span></span>

<span data-ttu-id="fafff-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="fafff-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="fafff-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fafff-118">Parameter</span></span> | <span data-ttu-id="fafff-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fafff-119">Type</span></span>   | <span data-ttu-id="fafff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fafff-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fafff-121">ponto</span><span class="sxs-lookup"><span data-stu-id="fafff-121">Period</span></span>    | <span data-ttu-id="fafff-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fafff-122">string</span></span> | <span data-ttu-id="fafff-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fafff-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fafff-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="fafff-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fafff-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fafff-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fafff-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fafff-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fafff-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fafff-127">Request headers</span></span>

| <span data-ttu-id="fafff-128">Nome</span><span class="sxs-lookup"><span data-stu-id="fafff-128">Name</span></span>          | <span data-ttu-id="fafff-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fafff-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fafff-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="fafff-130">Authorization</span></span> | <span data-ttu-id="fafff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fafff-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fafff-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fafff-133">if-none-match</span></span> | <span data-ttu-id="fafff-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="fafff-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="fafff-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fafff-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fafff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fafff-136">Response</span></span>

<span data-ttu-id="fafff-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="fafff-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fafff-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="fafff-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fafff-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fafff-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="fafff-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="fafff-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fafff-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="fafff-141">Report Refresh Date</span></span>
- <span data-ttu-id="fafff-142">Enviar</span><span class="sxs-lookup"><span data-stu-id="fafff-142">send</span></span>
- <span data-ttu-id="fafff-143">Receber</span><span class="sxs-lookup"><span data-stu-id="fafff-143">Receive</span></span>
- <span data-ttu-id="fafff-144">Ler</span><span class="sxs-lookup"><span data-stu-id="fafff-144">Read</span></span>
- <span data-ttu-id="fafff-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="fafff-145">Report Date</span></span>
- <span data-ttu-id="fafff-146">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="fafff-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fafff-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fafff-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fafff-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fafff-148">Request</span></span>

<span data-ttu-id="fafff-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fafff-149">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fafff-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fafff-150">Response</span></span>

<span data-ttu-id="fafff-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fafff-151">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fafff-152">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="fafff-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```
