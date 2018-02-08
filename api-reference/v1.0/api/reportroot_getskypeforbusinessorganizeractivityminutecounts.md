# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="47c1c-101">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="47c1c-101">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="47c1c-102">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="47c1c-102">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="47c1c-103">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="47c1c-103">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="47c1c-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="47c1c-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="47c1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47c1c-105">Permissions</span></span>

<span data-ttu-id="47c1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47c1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="47c1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47c1c-108">Permission type</span></span>                        | <span data-ttu-id="47c1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47c1c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="47c1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47c1c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="47c1c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47c1c-111">Not supported.</span></span>                           |
| <span data-ttu-id="47c1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47c1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47c1c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47c1c-113">Not supported.</span></span>                           |
| <span data-ttu-id="47c1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47c1c-114">Application</span></span>                            | <span data-ttu-id="47c1c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47c1c-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="47c1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47c1c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="47c1c-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="47c1c-117">Request parameters</span></span>

<span data-ttu-id="47c1c-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="47c1c-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="47c1c-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47c1c-119">Parameter</span></span> | <span data-ttu-id="47c1c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="47c1c-120">Type</span></span>   | <span data-ttu-id="47c1c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="47c1c-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="47c1c-122">ponto</span><span class="sxs-lookup"><span data-stu-id="47c1c-122">period</span></span>    | <span data-ttu-id="47c1c-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c1c-123">string</span></span> | <span data-ttu-id="47c1c-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="47c1c-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="47c1c-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="47c1c-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="47c1c-126">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="47c1c-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="47c1c-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47c1c-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="47c1c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47c1c-128">Request headers</span></span>

| <span data-ttu-id="47c1c-129">Nome</span><span class="sxs-lookup"><span data-stu-id="47c1c-129">Name</span></span>          | <span data-ttu-id="47c1c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="47c1c-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="47c1c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="47c1c-131">Authorization</span></span> | <span data-ttu-id="47c1c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47c1c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47c1c-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="47c1c-134">If-None-Match</span></span> | <span data-ttu-id="47c1c-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="47c1c-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="47c1c-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="47c1c-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="47c1c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c1c-137">Response</span></span>

<span data-ttu-id="47c1c-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="47c1c-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="47c1c-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="47c1c-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="47c1c-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="47c1c-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="47c1c-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="47c1c-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="47c1c-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="47c1c-142">Report Refresh Date</span></span>
- <span data-ttu-id="47c1c-143">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="47c1c-143">Report Date</span></span>
- <span data-ttu-id="47c1c-144">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="47c1c-144">Report Period</span></span>
- <span data-ttu-id="47c1c-145">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="47c1c-145">Audio/Video</span></span>
- <span data-ttu-id="47c1c-146">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="47c1c-146">Dial-in Microsoft</span></span>
- <span data-ttu-id="47c1c-147">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="47c1c-147">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="47c1c-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47c1c-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="47c1c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47c1c-149">Request</span></span>

<span data-ttu-id="47c1c-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47c1c-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="47c1c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c1c-151">Response</span></span>

<span data-ttu-id="47c1c-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47c1c-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="47c1c-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="47c1c-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```
