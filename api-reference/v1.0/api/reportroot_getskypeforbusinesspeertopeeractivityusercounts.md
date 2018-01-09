# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="1dfed-101">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1dfed-101">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="1dfed-102">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="1dfed-102">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="1dfed-103">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="1dfed-103">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="1dfed-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business]((https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)).</span><span class="sxs-lookup"><span data-stu-id="1dfed-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity]((https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dfed-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dfed-105">Permissions</span></span>

<span data-ttu-id="1dfed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1dfed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="1dfed-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dfed-108">Permission type</span></span>                        | <span data-ttu-id="1dfed-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dfed-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1dfed-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dfed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dfed-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dfed-111">Not supported.</span></span>                           |
| <span data-ttu-id="1dfed-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dfed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dfed-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dfed-113">Not supported.</span></span>                           |
| <span data-ttu-id="1dfed-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfed-114">Application</span></span>                            | <span data-ttu-id="1dfed-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dfed-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1dfed-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dfed-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="1dfed-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="1dfed-117">Request parameters</span></span>

<span data-ttu-id="1dfed-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="1dfed-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="1dfed-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1dfed-119">Parameter</span></span> | <span data-ttu-id="1dfed-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dfed-120">Type</span></span>   | <span data-ttu-id="1dfed-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dfed-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1dfed-122">ponto</span><span class="sxs-lookup"><span data-stu-id="1dfed-122">Period</span></span>    | <span data-ttu-id="1dfed-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dfed-123">string</span></span> | <span data-ttu-id="1dfed-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1dfed-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1dfed-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1dfed-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1dfed-126">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1dfed-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1dfed-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dfed-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1dfed-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfed-128">Request headers</span></span>

| <span data-ttu-id="1dfed-129">Nome</span><span class="sxs-lookup"><span data-stu-id="1dfed-129">Name</span></span>          | <span data-ttu-id="1dfed-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dfed-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1dfed-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dfed-131">Authorization</span></span> | <span data-ttu-id="1dfed-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dfed-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dfed-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1dfed-134">if-none-match</span></span> | <span data-ttu-id="1dfed-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="1dfed-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="1dfed-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1dfed-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1dfed-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dfed-137">Response</span></span>

<span data-ttu-id="1dfed-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1dfed-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1dfed-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1dfed-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1dfed-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1dfed-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="1dfed-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1dfed-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1dfed-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1dfed-142">Report Refresh Date</span></span>
- <span data-ttu-id="1dfed-143">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1dfed-143">Report Date</span></span>
- <span data-ttu-id="1dfed-144">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1dfed-144">Report Period</span></span>
- <span data-ttu-id="1dfed-145">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="1dfed-145">IM Address</span></span>
- <span data-ttu-id="1dfed-146">Áudio</span><span class="sxs-lookup"><span data-stu-id="1dfed-146">Audio</span></span>
- <span data-ttu-id="1dfed-147">Vídeo</span><span class="sxs-lookup"><span data-stu-id="1dfed-147">Video</span></span>
- <span data-ttu-id="1dfed-148">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1dfed-148">App sharing</span></span>
- <span data-ttu-id="1dfed-149">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="1dfed-149">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="1dfed-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dfed-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1dfed-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfed-151">Request</span></span>

<span data-ttu-id="1dfed-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dfed-152">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="1dfed-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dfed-153">Response</span></span>

<span data-ttu-id="1dfed-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1dfed-154">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1dfed-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1dfed-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
