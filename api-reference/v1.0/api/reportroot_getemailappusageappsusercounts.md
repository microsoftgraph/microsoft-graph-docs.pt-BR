# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="227d5-101">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="227d5-101">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="227d5-102">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="227d5-102">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="227d5-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="227d5-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="227d5-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="227d5-104">Permissions</span></span>

<span data-ttu-id="227d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="227d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="227d5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="227d5-107">Permission type</span></span>                        | <span data-ttu-id="227d5-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="227d5-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="227d5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="227d5-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="227d5-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="227d5-110">Not supported.</span></span>                           |
| <span data-ttu-id="227d5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="227d5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="227d5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="227d5-112">Not supported.</span></span>                           |
| <span data-ttu-id="227d5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="227d5-113">Application</span></span>                            | <span data-ttu-id="227d5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="227d5-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="227d5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="227d5-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="227d5-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="227d5-116">Request parameters</span></span>

<span data-ttu-id="227d5-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="227d5-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="227d5-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="227d5-118">Parameter</span></span> | <span data-ttu-id="227d5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="227d5-119">Type</span></span>   | <span data-ttu-id="227d5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="227d5-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="227d5-121">ponto</span><span class="sxs-lookup"><span data-stu-id="227d5-121">period</span></span>    | <span data-ttu-id="227d5-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="227d5-122">string</span></span> | <span data-ttu-id="227d5-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="227d5-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="227d5-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="227d5-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="227d5-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="227d5-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="227d5-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227d5-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="227d5-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="227d5-127">Request headers</span></span>

| <span data-ttu-id="227d5-128">Nome</span><span class="sxs-lookup"><span data-stu-id="227d5-128">Name</span></span>          | <span data-ttu-id="227d5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="227d5-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="227d5-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="227d5-130">Authorization</span></span> | <span data-ttu-id="227d5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227d5-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="227d5-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="227d5-133">If-None-Match</span></span> | <span data-ttu-id="227d5-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="227d5-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="227d5-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="227d5-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="227d5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="227d5-136">Response</span></span>

<span data-ttu-id="227d5-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="227d5-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="227d5-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="227d5-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="227d5-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="227d5-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="227d5-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="227d5-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="227d5-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="227d5-141">Report Refresh Date</span></span>
- <span data-ttu-id="227d5-142">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="227d5-142">Mail For Mac</span></span>
- <span data-ttu-id="227d5-143">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="227d5-143">Outlook For Mac</span></span>
- <span data-ttu-id="227d5-144">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="227d5-144">Outlook For Windows</span></span>
- <span data-ttu-id="227d5-145">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="227d5-145">Outlook For Mobile</span></span>
- <span data-ttu-id="227d5-146">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="227d5-146">Other For Mobile</span></span>
- <span data-ttu-id="227d5-147">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="227d5-147">Outlook For Web</span></span>
- <span data-ttu-id="227d5-148">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="227d5-148">POP3 App</span></span>
- <span data-ttu-id="227d5-149">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="227d5-149">IMAP4 App</span></span>
- <span data-ttu-id="227d5-150">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="227d5-150">SMTP App</span></span>
- <span data-ttu-id="227d5-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="227d5-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="227d5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="227d5-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="227d5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="227d5-153">Request</span></span>

<span data-ttu-id="227d5-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="227d5-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="227d5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="227d5-155">Response</span></span>

<span data-ttu-id="227d5-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="227d5-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="227d5-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="227d5-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
