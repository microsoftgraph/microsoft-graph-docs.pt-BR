# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="a1d7d-101">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a1d7d-101">reportRoot: getSkypeForBusinessActivityCounts</span></span>

<span data-ttu-id="a1d7d-102">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-102">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="a1d7d-103">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-103">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="a1d7d-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business]((https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)).</span><span class="sxs-lookup"><span data-stu-id="a1d7d-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity]((https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1d7d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1d7d-105">Permissions</span></span>

<span data-ttu-id="a1d7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1d7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a1d7d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1d7d-108">Permission type</span></span>                        | <span data-ttu-id="a1d7d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1d7d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a1d7d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1d7d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1d7d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-111">Not supported.</span></span>                           |
| <span data-ttu-id="a1d7d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1d7d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1d7d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-113">Not supported.</span></span>                           |
| <span data-ttu-id="a1d7d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1d7d-114">Application</span></span>                            | <span data-ttu-id="a1d7d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1d7d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a1d7d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d7d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="a1d7d-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="a1d7d-117">Request parameters</span></span>

<span data-ttu-id="a1d7d-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="a1d7d-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a1d7d-119">Parameter</span></span> | <span data-ttu-id="a1d7d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1d7d-120">Type</span></span>   | <span data-ttu-id="a1d7d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d7d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a1d7d-122">ponto</span><span class="sxs-lookup"><span data-stu-id="a1d7d-122">Period</span></span>    | <span data-ttu-id="a1d7d-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1d7d-123">string</span></span> | <span data-ttu-id="a1d7d-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a1d7d-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a1d7d-126">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a1d7d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a1d7d-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d7d-128">Request headers</span></span>

| <span data-ttu-id="a1d7d-129">Nome</span><span class="sxs-lookup"><span data-stu-id="a1d7d-129">Name</span></span>          | <span data-ttu-id="a1d7d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d7d-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a1d7d-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1d7d-131">Authorization</span></span> | <span data-ttu-id="a1d7d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1d7d-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a1d7d-134">if-none-match</span></span> | <span data-ttu-id="a1d7d-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="a1d7d-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a1d7d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d7d-137">Response</span></span>

<span data-ttu-id="a1d7d-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a1d7d-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a1d7d-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="a1d7d-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a1d7d-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a1d7d-142">Report Refresh Date</span></span>
- <span data-ttu-id="a1d7d-143">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a1d7d-143">Report Date</span></span>
- <span data-ttu-id="a1d7d-144">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a1d7d-144">Report Period</span></span>
- <span data-ttu-id="a1d7d-145">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="a1d7d-145">Peer-to-peer</span></span>
- <span data-ttu-id="a1d7d-146">Organizadas</span><span class="sxs-lookup"><span data-stu-id="a1d7d-146">Organized</span></span>
- <span data-ttu-id="a1d7d-147">Participadas</span><span class="sxs-lookup"><span data-stu-id="a1d7d-147">Participated</span></span>

## <a name="example"></a><span data-ttu-id="a1d7d-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1d7d-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a1d7d-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d7d-149">Request</span></span>

<span data-ttu-id="a1d7d-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-150">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a1d7d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d7d-151">Response</span></span>

<span data-ttu-id="a1d7d-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-152">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a1d7d-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a1d7d-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```
