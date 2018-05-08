# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="9f94e-101">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="9f94e-101">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="9f94e-102">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="9f94e-102">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="9f94e-103">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="9f94e-103">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="9f94e-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="9f94e-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f94e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f94e-105">Permissions</span></span>

<span data-ttu-id="9f94e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f94e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="9f94e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f94e-108">Permission type</span></span>                        | <span data-ttu-id="9f94e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f94e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9f94e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f94e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f94e-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f94e-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9f94e-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f94e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f94e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f94e-113">Not supported.</span></span>                           |
| <span data-ttu-id="9f94e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f94e-114">Application</span></span>                            | <span data-ttu-id="9f94e-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f94e-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9f94e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f94e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="9f94e-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="9f94e-117">Request parameters</span></span>

<span data-ttu-id="9f94e-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9f94e-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9f94e-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9f94e-119">Parameter</span></span> | <span data-ttu-id="9f94e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f94e-120">Type</span></span>   | <span data-ttu-id="9f94e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f94e-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9f94e-122">ponto</span><span class="sxs-lookup"><span data-stu-id="9f94e-122">period</span></span>    | <span data-ttu-id="9f94e-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f94e-123">string</span></span> | <span data-ttu-id="9f94e-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9f94e-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9f94e-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9f94e-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9f94e-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9f94e-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9f94e-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f94e-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9f94e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f94e-128">Request headers</span></span>

| <span data-ttu-id="9f94e-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9f94e-129">Name</span></span>          | <span data-ttu-id="9f94e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f94e-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9f94e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f94e-131">Authorization</span></span> | <span data-ttu-id="9f94e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f94e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9f94e-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9f94e-134">If-None-Match</span></span> | <span data-ttu-id="9f94e-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="9f94e-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9f94e-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f94e-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9f94e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f94e-137">Response</span></span>

<span data-ttu-id="9f94e-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9f94e-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9f94e-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9f94e-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9f94e-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9f94e-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9f94e-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9f94e-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9f94e-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9f94e-142">Report Refresh Date</span></span>
- <span data-ttu-id="9f94e-143">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="9f94e-143">Site Type</span></span>
- <span data-ttu-id="9f94e-144">Total</span><span class="sxs-lookup"><span data-stu-id="9f94e-144">Total</span></span>
- <span data-ttu-id="9f94e-145">Ativo</span><span class="sxs-lookup"><span data-stu-id="9f94e-145">Active</span></span>
- <span data-ttu-id="9f94e-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="9f94e-146">Report Date</span></span>
- <span data-ttu-id="9f94e-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9f94e-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9f94e-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f94e-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9f94e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f94e-149">Request</span></span>

<span data-ttu-id="9f94e-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f94e-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9f94e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f94e-151">Response</span></span>

<span data-ttu-id="9f94e-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f94e-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9f94e-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9f94e-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
