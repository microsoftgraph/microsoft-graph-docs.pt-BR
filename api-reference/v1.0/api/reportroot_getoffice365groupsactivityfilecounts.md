# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="48094-101">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="48094-101">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="48094-102">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="48094-102">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="48094-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365]((https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)).</span><span class="sxs-lookup"><span data-stu-id="48094-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups]((https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)).</span></span>

## <a name="permissions"></a><span data-ttu-id="48094-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="48094-104">Permissions</span></span>

<span data-ttu-id="48094-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="48094-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48094-107">Permission type</span></span>                        | <span data-ttu-id="48094-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48094-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="48094-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48094-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="48094-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48094-110">Not supported.</span></span>                           |
| <span data-ttu-id="48094-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48094-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48094-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48094-112">Not supported.</span></span>                           |
| <span data-ttu-id="48094-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48094-113">Application</span></span>                            | <span data-ttu-id="48094-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48094-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="48094-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48094-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="48094-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="48094-116">Request parameters</span></span>

<span data-ttu-id="48094-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="48094-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="48094-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="48094-118">Parameter</span></span> | <span data-ttu-id="48094-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="48094-119">Type</span></span>   | <span data-ttu-id="48094-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="48094-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="48094-121">ponto</span><span class="sxs-lookup"><span data-stu-id="48094-121">Period</span></span>    | <span data-ttu-id="48094-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48094-122">string</span></span> | <span data-ttu-id="48094-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="48094-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="48094-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="48094-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="48094-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="48094-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="48094-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48094-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="48094-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48094-127">Request headers</span></span>

| <span data-ttu-id="48094-128">Nome</span><span class="sxs-lookup"><span data-stu-id="48094-128">Name</span></span>          | <span data-ttu-id="48094-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="48094-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="48094-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="48094-130">Authorization</span></span> | <span data-ttu-id="48094-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48094-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="48094-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="48094-133">if-none-match</span></span> | <span data-ttu-id="48094-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="48094-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="48094-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="48094-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="48094-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="48094-136">Response</span></span>

<span data-ttu-id="48094-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="48094-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="48094-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="48094-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="48094-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="48094-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="48094-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="48094-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="48094-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="48094-141">Report Refresh Date</span></span>
- <span data-ttu-id="48094-142">Total</span><span class="sxs-lookup"><span data-stu-id="48094-142">total</span></span>
- <span data-ttu-id="48094-143">Ativo</span><span class="sxs-lookup"><span data-stu-id="48094-143">Active</span></span>
- <span data-ttu-id="48094-144">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="48094-144">Report Date</span></span>
- <span data-ttu-id="48094-145">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="48094-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="48094-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48094-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="48094-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48094-147">Request</span></span>

<span data-ttu-id="48094-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48094-148">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="48094-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="48094-149">Response</span></span>

<span data-ttu-id="48094-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48094-150">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="48094-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="48094-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
