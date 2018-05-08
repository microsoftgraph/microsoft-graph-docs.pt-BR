# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="15683-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="15683-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="15683-102">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="15683-102">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="15683-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="15683-103">Permissions</span></span>

<span data-ttu-id="15683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="15683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="15683-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15683-106">Permission type</span></span>                        | <span data-ttu-id="15683-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15683-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="15683-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15683-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="15683-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15683-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="15683-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15683-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15683-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15683-111">Not supported.</span></span>                           |
| <span data-ttu-id="15683-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15683-112">Application</span></span>                            | <span data-ttu-id="15683-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15683-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="15683-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15683-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="15683-115">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="15683-115">Request parameters</span></span>

<span data-ttu-id="15683-116">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="15683-116">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="15683-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="15683-117">Parameter</span></span> | <span data-ttu-id="15683-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="15683-118">Type</span></span>   | <span data-ttu-id="15683-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="15683-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="15683-120">ponto</span><span class="sxs-lookup"><span data-stu-id="15683-120">period</span></span>    | <span data-ttu-id="15683-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15683-121">string</span></span> | <span data-ttu-id="15683-122">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="15683-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="15683-123">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="15683-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="15683-124">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="15683-124">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="15683-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15683-125">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="15683-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15683-126">Request headers</span></span>

| <span data-ttu-id="15683-127">Nome</span><span class="sxs-lookup"><span data-stu-id="15683-127">Name</span></span>          | <span data-ttu-id="15683-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="15683-128">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="15683-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="15683-129">Authorization</span></span> | <span data-ttu-id="15683-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15683-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="15683-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="15683-132">Response</span></span>

<span data-ttu-id="15683-133">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="15683-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="15683-134">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="15683-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="15683-135">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="15683-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="15683-136">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="15683-136">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="15683-137">Data de Atualização do Relatório</span><span class="sxs-lookup"><span data-stu-id="15683-137">Report Refresh Date</span></span>
- <span data-ttu-id="15683-138">Web</span><span class="sxs-lookup"><span data-stu-id="15683-138">Web</span></span>
- <span data-ttu-id="15683-139">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="15683-139">Windows Phone</span></span>
- <span data-ttu-id="15683-140">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="15683-140">Android Phone</span></span>
- <span data-ttu-id="15683-141">iOS</span><span class="sxs-lookup"><span data-stu-id="15683-141">iOS</span></span>
- <span data-ttu-id="15683-142">Mac</span><span class="sxs-lookup"><span data-stu-id="15683-142">Mac</span></span>
- <span data-ttu-id="15683-143">Windows</span><span class="sxs-lookup"><span data-stu-id="15683-143">Windows</span></span>
- <span data-ttu-id="15683-144">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="15683-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="15683-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15683-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="15683-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15683-146">Request</span></span>

<span data-ttu-id="15683-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15683-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="15683-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="15683-148">Response</span></span>

<span data-ttu-id="15683-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15683-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="15683-150">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="15683-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
