# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="5d403-101">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="5d403-101">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="5d403-102">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="5d403-102">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="5d403-103">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="5d403-103">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="5d403-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="5d403-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d403-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d403-105">Permissions</span></span>

<span data-ttu-id="5d403-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d403-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5d403-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d403-108">Permission type</span></span>                        | <span data-ttu-id="5d403-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d403-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5d403-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d403-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d403-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d403-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5d403-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d403-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d403-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d403-113">Not supported.</span></span>                           |
| <span data-ttu-id="5d403-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d403-114">Application</span></span>                            | <span data-ttu-id="5d403-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d403-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5d403-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d403-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="5d403-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="5d403-117">Request parameters</span></span>

<span data-ttu-id="5d403-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5d403-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5d403-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5d403-119">Parameter</span></span> | <span data-ttu-id="5d403-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d403-120">Type</span></span>   | <span data-ttu-id="5d403-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d403-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5d403-122">ponto</span><span class="sxs-lookup"><span data-stu-id="5d403-122">period</span></span>    | <span data-ttu-id="5d403-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d403-123">string</span></span> | <span data-ttu-id="5d403-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5d403-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5d403-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5d403-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5d403-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5d403-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5d403-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d403-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5d403-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d403-128">Request headers</span></span>

| <span data-ttu-id="5d403-129">Nome</span><span class="sxs-lookup"><span data-stu-id="5d403-129">Name</span></span>          | <span data-ttu-id="5d403-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d403-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5d403-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d403-131">Authorization</span></span> | <span data-ttu-id="5d403-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d403-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5d403-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5d403-134">If-None-Match</span></span> | <span data-ttu-id="5d403-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5d403-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5d403-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d403-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5d403-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d403-137">Response</span></span>

<span data-ttu-id="5d403-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5d403-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5d403-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5d403-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5d403-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5d403-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5d403-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5d403-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5d403-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5d403-142">Report Refresh Date</span></span>
- <span data-ttu-id="5d403-143">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5d403-143">Report Date</span></span>
- <span data-ttu-id="5d403-144">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5d403-144">Report Period</span></span>
- <span data-ttu-id="5d403-145">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="5d403-145">IM</span></span>
- <span data-ttu-id="5d403-146">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="5d403-146">Audio/Video</span></span>
- <span data-ttu-id="5d403-147">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="5d403-147">App Sharing</span></span>
- <span data-ttu-id="5d403-148">Web</span><span class="sxs-lookup"><span data-stu-id="5d403-148">Web</span></span>
- <span data-ttu-id="5d403-149">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="5d403-149">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="5d403-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d403-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5d403-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d403-151">Request</span></span>

<span data-ttu-id="5d403-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d403-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5d403-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d403-153">Response</span></span>

<span data-ttu-id="5d403-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d403-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5d403-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5d403-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```
