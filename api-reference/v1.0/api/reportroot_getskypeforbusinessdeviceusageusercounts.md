# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="82c32-101">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="82c32-101">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="82c32-102">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="82c32-102">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="82c32-103">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="82c32-103">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="82c32-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="82c32-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="82c32-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="82c32-105">Permissions</span></span>

<span data-ttu-id="82c32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="82c32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="82c32-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82c32-108">Permission type</span></span>                        | <span data-ttu-id="82c32-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82c32-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="82c32-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82c32-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82c32-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="82c32-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="82c32-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82c32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82c32-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c32-113">Not supported.</span></span>                           |
| <span data-ttu-id="82c32-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82c32-114">Application</span></span>                            | <span data-ttu-id="82c32-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="82c32-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="82c32-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82c32-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="82c32-117">Parâmetros da função</span><span class="sxs-lookup"><span data-stu-id="82c32-117">Function parameters</span></span>

<span data-ttu-id="82c32-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="82c32-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="82c32-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="82c32-119">Parameter</span></span> | <span data-ttu-id="82c32-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="82c32-120">Type</span></span>   | <span data-ttu-id="82c32-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c32-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="82c32-122">ponto</span><span class="sxs-lookup"><span data-stu-id="82c32-122">period</span></span>    | <span data-ttu-id="82c32-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82c32-123">string</span></span> | <span data-ttu-id="82c32-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="82c32-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="82c32-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="82c32-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="82c32-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="82c32-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="82c32-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82c32-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="82c32-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82c32-128">Request headers</span></span>

| <span data-ttu-id="82c32-129">Nome</span><span class="sxs-lookup"><span data-stu-id="82c32-129">Name</span></span>          | <span data-ttu-id="82c32-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c32-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="82c32-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="82c32-131">Authorization</span></span> | <span data-ttu-id="82c32-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82c32-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="82c32-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="82c32-134">If-None-Match</span></span> | <span data-ttu-id="82c32-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="82c32-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="82c32-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="82c32-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="82c32-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c32-137">Response</span></span>

<span data-ttu-id="82c32-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="82c32-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="82c32-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="82c32-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="82c32-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="82c32-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="82c32-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="82c32-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="82c32-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="82c32-142">Report Refresh Date</span></span>
- <span data-ttu-id="82c32-143">Windows</span><span class="sxs-lookup"><span data-stu-id="82c32-143">Windows</span></span>
- <span data-ttu-id="82c32-144">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="82c32-144">Windows Phone</span></span>
- <span data-ttu-id="82c32-145">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="82c32-145">Android Phone</span></span>
- <span data-ttu-id="82c32-146">iPhone</span><span class="sxs-lookup"><span data-stu-id="82c32-146">iPhone</span></span>
- <span data-ttu-id="82c32-147">iPad</span><span class="sxs-lookup"><span data-stu-id="82c32-147">iPad</span></span>
- <span data-ttu-id="82c32-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="82c32-148">Report Date</span></span>
- <span data-ttu-id="82c32-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="82c32-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="82c32-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82c32-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="82c32-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82c32-151">Request</span></span>

<span data-ttu-id="82c32-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c32-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="82c32-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c32-153">Response</span></span>

<span data-ttu-id="82c32-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="82c32-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="82c32-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="82c32-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
