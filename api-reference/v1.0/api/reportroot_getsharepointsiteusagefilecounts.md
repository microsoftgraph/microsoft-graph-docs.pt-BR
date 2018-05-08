# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="f246d-101">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="f246d-101">reportRoot: getSharePointSiteUsageFileCounts</span></span>

<span data-ttu-id="f246d-102">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="f246d-102">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="f246d-103">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="f246d-103">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="f246d-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="f246d-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="f246d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f246d-105">Permissions</span></span>

<span data-ttu-id="f246d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f246d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f246d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f246d-108">Permission type</span></span>                        | <span data-ttu-id="f246d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f246d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f246d-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f246d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f246d-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f246d-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f246d-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f246d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f246d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f246d-113">Not supported.</span></span>                           |
| <span data-ttu-id="f246d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f246d-114">Application</span></span>                            | <span data-ttu-id="f246d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f246d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f246d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f246d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="f246d-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="f246d-117">Request parameters</span></span>

<span data-ttu-id="f246d-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f246d-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f246d-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f246d-119">Parameter</span></span> | <span data-ttu-id="f246d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f246d-120">Type</span></span>   | <span data-ttu-id="f246d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f246d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f246d-122">ponto</span><span class="sxs-lookup"><span data-stu-id="f246d-122">period</span></span>    | <span data-ttu-id="f246d-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f246d-123">string</span></span> | <span data-ttu-id="f246d-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f246d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f246d-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f246d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f246d-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f246d-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f246d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f246d-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f246d-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f246d-128">Request headers</span></span>

| <span data-ttu-id="f246d-129">Nome</span><span class="sxs-lookup"><span data-stu-id="f246d-129">Name</span></span>          | <span data-ttu-id="f246d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f246d-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f246d-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f246d-131">Authorization</span></span> | <span data-ttu-id="f246d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f246d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f246d-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f246d-134">If-None-Match</span></span> | <span data-ttu-id="f246d-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="f246d-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f246d-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f246d-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f246d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f246d-137">Response</span></span>

<span data-ttu-id="f246d-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f246d-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f246d-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f246d-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f246d-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f246d-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f246d-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f246d-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f246d-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f246d-142">Report Refresh Date</span></span>
- <span data-ttu-id="f246d-143">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="f246d-143">Site Type</span></span>
- <span data-ttu-id="f246d-144">Total</span><span class="sxs-lookup"><span data-stu-id="f246d-144">Total</span></span>
- <span data-ttu-id="f246d-145">Ativo</span><span class="sxs-lookup"><span data-stu-id="f246d-145">Active</span></span>
- <span data-ttu-id="f246d-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="f246d-146">Report Date</span></span>
- <span data-ttu-id="f246d-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f246d-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f246d-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f246d-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f246d-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f246d-149">Request</span></span>

<span data-ttu-id="f246d-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f246d-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f246d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f246d-151">Response</span></span>

<span data-ttu-id="f246d-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f246d-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f246d-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f246d-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
