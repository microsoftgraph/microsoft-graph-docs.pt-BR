# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="9bbaf-101">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="9bbaf-101">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="9bbaf-102">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-102">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="9bbaf-103">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-103">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="9bbaf-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes]((https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)).</span><span class="sxs-lookup"><span data-stu-id="9bbaf-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used]((https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)).</span></span>

## <a name="permissions"></a><span data-ttu-id="9bbaf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bbaf-105">Permissions</span></span>

<span data-ttu-id="9bbaf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9bbaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="9bbaf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bbaf-108">Permission type</span></span>                        | <span data-ttu-id="9bbaf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bbaf-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9bbaf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bbaf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9bbaf-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-111">Not supported.</span></span>                           |
| <span data-ttu-id="9bbaf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bbaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bbaf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-113">Not supported.</span></span>                           |
| <span data-ttu-id="9bbaf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bbaf-114">Application</span></span>                            | <span data-ttu-id="9bbaf-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bbaf-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9bbaf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bbaf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="9bbaf-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="9bbaf-117">Request parameters</span></span>

<span data-ttu-id="9bbaf-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="9bbaf-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9bbaf-119">Parameter</span></span> | <span data-ttu-id="9bbaf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bbaf-120">Type</span></span>   | <span data-ttu-id="9bbaf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bbaf-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9bbaf-122">ponto</span><span class="sxs-lookup"><span data-stu-id="9bbaf-122">Period</span></span>    | <span data-ttu-id="9bbaf-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bbaf-123">string</span></span> | <span data-ttu-id="9bbaf-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9bbaf-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9bbaf-126">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9bbaf-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9bbaf-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bbaf-128">Request headers</span></span>

| <span data-ttu-id="9bbaf-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9bbaf-129">Name</span></span>          | <span data-ttu-id="9bbaf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bbaf-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9bbaf-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bbaf-131">Authorization</span></span> | <span data-ttu-id="9bbaf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bbaf-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9bbaf-134">if-none-match</span></span> | <span data-ttu-id="9bbaf-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="9bbaf-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9bbaf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bbaf-137">Response</span></span>

<span data-ttu-id="9bbaf-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9bbaf-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9bbaf-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="9bbaf-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9bbaf-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9bbaf-142">Report Refresh Date</span></span>
- <span data-ttu-id="9bbaf-143">Windows</span><span class="sxs-lookup"><span data-stu-id="9bbaf-143">Windows</span></span>
- <span data-ttu-id="9bbaf-144">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="9bbaf-144">Windows Phone</span></span>
- <span data-ttu-id="9bbaf-145">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="9bbaf-145">Office for Android Phone</span></span>
- <span data-ttu-id="9bbaf-146">iPhone</span><span class="sxs-lookup"><span data-stu-id="9bbaf-146">iPhone channel</span></span>
- <span data-ttu-id="9bbaf-147">iPad</span><span class="sxs-lookup"><span data-stu-id="9bbaf-147">iPad channel</span></span>
- <span data-ttu-id="9bbaf-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9bbaf-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9bbaf-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bbaf-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9bbaf-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bbaf-150">Request</span></span>

<span data-ttu-id="9bbaf-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-151">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9bbaf-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bbaf-152">Response</span></span>

<span data-ttu-id="9bbaf-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-153">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9bbaf-154">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9bbaf-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```
