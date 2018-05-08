# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="7cebf-101">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7cebf-101">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="7cebf-102">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="7cebf-102">Get the trend in the number of active users.</span></span> <span data-ttu-id="7cebf-103">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="7cebf-103">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="7cebf-104">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="7cebf-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cebf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cebf-105">Permissions</span></span>

<span data-ttu-id="7cebf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cebf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7cebf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cebf-108">Permission type</span></span>                        | <span data-ttu-id="7cebf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cebf-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7cebf-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cebf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cebf-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cebf-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7cebf-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cebf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cebf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cebf-113">Not supported.</span></span>                           |
| <span data-ttu-id="7cebf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cebf-114">Application</span></span>                            | <span data-ttu-id="7cebf-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cebf-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7cebf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cebf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="7cebf-117">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="7cebf-117">Request parameters</span></span>

<span data-ttu-id="7cebf-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7cebf-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7cebf-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7cebf-119">Parameter</span></span> | <span data-ttu-id="7cebf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cebf-120">Type</span></span>   | <span data-ttu-id="7cebf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cebf-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7cebf-122">ponto</span><span class="sxs-lookup"><span data-stu-id="7cebf-122">period</span></span>    | <span data-ttu-id="7cebf-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cebf-123">string</span></span> | <span data-ttu-id="7cebf-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7cebf-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7cebf-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7cebf-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7cebf-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7cebf-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7cebf-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cebf-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7cebf-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cebf-128">Request headers</span></span>

| <span data-ttu-id="7cebf-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7cebf-129">Name</span></span>          | <span data-ttu-id="7cebf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cebf-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7cebf-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cebf-131">Authorization</span></span> | <span data-ttu-id="7cebf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cebf-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7cebf-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7cebf-134">If-None-Match</span></span> | <span data-ttu-id="7cebf-135">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="7cebf-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7cebf-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7cebf-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7cebf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cebf-137">Response</span></span>

<span data-ttu-id="7cebf-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7cebf-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7cebf-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7cebf-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7cebf-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7cebf-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7cebf-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7cebf-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7cebf-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7cebf-142">Report Refresh Date</span></span>
- <span data-ttu-id="7cebf-143">Página visitada</span><span class="sxs-lookup"><span data-stu-id="7cebf-143">Visited Page</span></span>
- <span data-ttu-id="7cebf-144">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="7cebf-144">Viewed Or Edited</span></span>
- <span data-ttu-id="7cebf-145">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="7cebf-145">Synced</span></span>
- <span data-ttu-id="7cebf-146">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="7cebf-146">Shared Internally</span></span>
- <span data-ttu-id="7cebf-147">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="7cebf-147">Shared Externally</span></span>
- <span data-ttu-id="7cebf-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="7cebf-148">Report Date</span></span>
- <span data-ttu-id="7cebf-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7cebf-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7cebf-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cebf-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7cebf-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cebf-151">Request</span></span>

<span data-ttu-id="7cebf-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cebf-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7cebf-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cebf-153">Response</span></span>

<span data-ttu-id="7cebf-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7cebf-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7cebf-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7cebf-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
