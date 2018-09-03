# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="43ed0-101">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="43ed0-101">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="43ed0-102">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43ed0-102">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="43ed0-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="43ed0-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="43ed0-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="43ed0-104">Permissions</span></span>

<span data-ttu-id="43ed0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43ed0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="43ed0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43ed0-107">Permission type</span></span>                        | <span data-ttu-id="43ed0-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43ed0-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="43ed0-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43ed0-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="43ed0-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43ed0-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="43ed0-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43ed0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43ed0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43ed0-112">Not supported.</span></span>                           |
| <span data-ttu-id="43ed0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43ed0-113">Application</span></span>                            | <span data-ttu-id="43ed0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43ed0-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="43ed0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43ed0-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="43ed0-116">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="43ed0-116">Function parameters</span></span>

<span data-ttu-id="43ed0-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="43ed0-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="43ed0-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="43ed0-118">Parameter</span></span> | <span data-ttu-id="43ed0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="43ed0-119">Type</span></span>   | <span data-ttu-id="43ed0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="43ed0-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="43ed0-121">ponto</span><span class="sxs-lookup"><span data-stu-id="43ed0-121">period</span></span>    | <span data-ttu-id="43ed0-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43ed0-122">string</span></span> | <span data-ttu-id="43ed0-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="43ed0-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="43ed0-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="43ed0-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="43ed0-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="43ed0-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="43ed0-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43ed0-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="43ed0-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43ed0-127">Request headers</span></span>

| <span data-ttu-id="43ed0-128">Nome</span><span class="sxs-lookup"><span data-stu-id="43ed0-128">Name</span></span>          | <span data-ttu-id="43ed0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="43ed0-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="43ed0-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="43ed0-130">Authorization</span></span> | <span data-ttu-id="43ed0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43ed0-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="43ed0-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="43ed0-133">If-None-Match</span></span> | <span data-ttu-id="43ed0-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="43ed0-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="43ed0-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="43ed0-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="43ed0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="43ed0-136">Response</span></span>

<span data-ttu-id="43ed0-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="43ed0-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="43ed0-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="43ed0-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="43ed0-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="43ed0-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="43ed0-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="43ed0-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="43ed0-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="43ed0-141">Report Refresh Date</span></span>
- <span data-ttu-id="43ed0-142">Web</span><span class="sxs-lookup"><span data-stu-id="43ed0-142">Web</span></span>
- <span data-ttu-id="43ed0-143">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="43ed0-143">Windows Phone</span></span>
- <span data-ttu-id="43ed0-144">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="43ed0-144">Android Phone</span></span>
- <span data-ttu-id="43ed0-145">iPhone</span><span class="sxs-lookup"><span data-stu-id="43ed0-145">iPhone</span></span>
- <span data-ttu-id="43ed0-146">iPad</span><span class="sxs-lookup"><span data-stu-id="43ed0-146">iPad</span></span>
- <span data-ttu-id="43ed0-147">Outro</span><span class="sxs-lookup"><span data-stu-id="43ed0-147">Other</span></span>
- <span data-ttu-id="43ed0-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="43ed0-148">Report Date</span></span>
- <span data-ttu-id="43ed0-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="43ed0-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="43ed0-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43ed0-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="43ed0-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43ed0-151">Request</span></span>

<span data-ttu-id="43ed0-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43ed0-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="43ed0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="43ed0-153">Response</span></span>

<span data-ttu-id="43ed0-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43ed0-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="43ed0-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="43ed0-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```
