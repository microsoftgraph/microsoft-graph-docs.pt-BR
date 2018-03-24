# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="d4482-101">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="d4482-101">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="d4482-102">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="d4482-102">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="d4482-103">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="d4482-103">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4482-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4482-104">Permissions</span></span>

<span data-ttu-id="d4482-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4482-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d4482-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4482-107">Permission type</span></span>                        | <span data-ttu-id="d4482-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4482-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d4482-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4482-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4482-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4482-110">Not supported.</span></span>                           |
| <span data-ttu-id="d4482-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4482-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4482-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4482-112">Not supported.</span></span>                           |
| <span data-ttu-id="d4482-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4482-113">Application</span></span>                            | <span data-ttu-id="d4482-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4482-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d4482-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4482-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="d4482-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="d4482-116">Request parameters</span></span>

<span data-ttu-id="d4482-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d4482-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="d4482-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4482-118">Parameter</span></span> | <span data-ttu-id="d4482-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4482-119">Type</span></span>   | <span data-ttu-id="d4482-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4482-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d4482-121">ponto</span><span class="sxs-lookup"><span data-stu-id="d4482-121">period</span></span>    | <span data-ttu-id="d4482-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4482-122">string</span></span> | <span data-ttu-id="d4482-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d4482-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d4482-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d4482-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d4482-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d4482-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d4482-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4482-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d4482-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4482-127">Request headers</span></span>

| <span data-ttu-id="d4482-128">Nome</span><span class="sxs-lookup"><span data-stu-id="d4482-128">Name</span></span>          | <span data-ttu-id="d4482-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4482-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d4482-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4482-130">Authorization</span></span> | <span data-ttu-id="d4482-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4482-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d4482-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4482-133">Response</span></span>

<span data-ttu-id="d4482-134">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d4482-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d4482-135">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d4482-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d4482-136">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d4482-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d4482-137">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="d4482-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d4482-138">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d4482-138">Report Refresh Date</span></span>
- <span data-ttu-id="d4482-139">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d4482-139">Report Date</span></span>
- <span data-ttu-id="d4482-140">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="d4482-140">Team Chat Messages</span></span>
- <span data-ttu-id="d4482-141">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="d4482-141">Private Chat Messages</span></span>
- <span data-ttu-id="d4482-142">Chamadas</span><span class="sxs-lookup"><span data-stu-id="d4482-142">API Calls</span></span>
- <span data-ttu-id="d4482-143">Reuniões</span><span class="sxs-lookup"><span data-stu-id="d4482-143">Suggested Meetings</span></span>
- <span data-ttu-id="d4482-144">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="d4482-144">Other Actions</span></span>
- <span data-ttu-id="d4482-145">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d4482-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d4482-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4482-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d4482-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4482-147">Request</span></span>

<span data-ttu-id="d4482-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4482-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d4482-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4482-149">Response</span></span>

<span data-ttu-id="d4482-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4482-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d4482-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d4482-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
