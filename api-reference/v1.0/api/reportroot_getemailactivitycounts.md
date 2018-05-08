# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="a8694-101">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a8694-101">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="a8694-102">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="a8694-102">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="a8694-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="a8694-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8694-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8694-104">Permissions</span></span>

<span data-ttu-id="a8694-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a8694-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8694-107">Permission type</span></span>                        | <span data-ttu-id="a8694-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8694-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a8694-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8694-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8694-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8694-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a8694-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8694-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8694-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8694-112">Not supported.</span></span>                           |
| <span data-ttu-id="a8694-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8694-113">Application</span></span>                            | <span data-ttu-id="a8694-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8694-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a8694-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8694-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="a8694-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="a8694-116">Request parameters</span></span>

<span data-ttu-id="a8694-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a8694-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a8694-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a8694-118">Parameter</span></span> | <span data-ttu-id="a8694-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8694-119">Type</span></span>   | <span data-ttu-id="a8694-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8694-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a8694-121">ponto</span><span class="sxs-lookup"><span data-stu-id="a8694-121">period</span></span>    | <span data-ttu-id="a8694-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8694-122">string</span></span> | <span data-ttu-id="a8694-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a8694-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a8694-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a8694-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a8694-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a8694-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a8694-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8694-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a8694-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8694-127">Request headers</span></span>

| <span data-ttu-id="a8694-128">Nome</span><span class="sxs-lookup"><span data-stu-id="a8694-128">Name</span></span>          | <span data-ttu-id="a8694-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8694-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a8694-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8694-130">Authorization</span></span> | <span data-ttu-id="a8694-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8694-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a8694-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a8694-133">If-None-Match</span></span> | <span data-ttu-id="a8694-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a8694-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a8694-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a8694-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a8694-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8694-136">Response</span></span>

<span data-ttu-id="a8694-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a8694-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a8694-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a8694-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a8694-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a8694-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a8694-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a8694-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a8694-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a8694-141">Report Refresh Date</span></span>
- <span data-ttu-id="a8694-142">Enviar</span><span class="sxs-lookup"><span data-stu-id="a8694-142">Send</span></span>
- <span data-ttu-id="a8694-143">Receber</span><span class="sxs-lookup"><span data-stu-id="a8694-143">Receive</span></span>
- <span data-ttu-id="a8694-144">Ler</span><span class="sxs-lookup"><span data-stu-id="a8694-144">Read</span></span>
- <span data-ttu-id="a8694-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a8694-145">Report Date</span></span>
- <span data-ttu-id="a8694-146">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a8694-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a8694-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8694-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a8694-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8694-148">Request</span></span>

<span data-ttu-id="a8694-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8694-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a8694-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8694-150">Response</span></span>

<span data-ttu-id="a8694-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8694-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a8694-152">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a8694-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
