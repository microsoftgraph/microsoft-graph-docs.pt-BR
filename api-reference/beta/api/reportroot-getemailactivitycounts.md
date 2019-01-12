---
title: 'reportRoot: getEmailActivityCounts'
description: Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4d4c076f3c40bb4c920a8f4f79cb9c410bfdb064
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931003"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="b6368-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b6368-103">reportRoot: getEmailActivityCounts</span></span>

> <span data-ttu-id="b6368-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6368-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6368-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6368-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6368-106">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="b6368-106">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="b6368-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="b6368-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6368-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6368-108">Permissions</span></span>

<span data-ttu-id="b6368-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6368-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6368-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6368-111">Permission type</span></span>                        | <span data-ttu-id="b6368-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6368-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b6368-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6368-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6368-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6368-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b6368-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6368-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6368-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6368-116">Not supported.</span></span>                           |
| <span data-ttu-id="b6368-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6368-117">Application</span></span>                            | <span data-ttu-id="b6368-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6368-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b6368-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6368-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b6368-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b6368-120">Function parameters</span></span>

<span data-ttu-id="b6368-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b6368-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b6368-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6368-122">Parameter</span></span> | <span data-ttu-id="b6368-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6368-123">Type</span></span>   | <span data-ttu-id="b6368-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6368-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b6368-125">ponto</span><span class="sxs-lookup"><span data-stu-id="b6368-125">period</span></span>    | <span data-ttu-id="b6368-126">string</span><span class="sxs-lookup"><span data-stu-id="b6368-126">string</span></span> | <span data-ttu-id="b6368-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b6368-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b6368-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b6368-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b6368-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b6368-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b6368-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6368-130">Required.</span></span> |

<span data-ttu-id="b6368-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6368-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b6368-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="b6368-132">The default output type is text/csv.</span></span> <span data-ttu-id="b6368-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="b6368-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6368-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6368-134">Request headers</span></span>

| <span data-ttu-id="b6368-135">Nome</span><span class="sxs-lookup"><span data-stu-id="b6368-135">Name</span></span>          | <span data-ttu-id="b6368-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6368-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b6368-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6368-137">Authorization</span></span> | <span data-ttu-id="b6368-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6368-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b6368-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6368-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b6368-141">CSV</span><span class="sxs-lookup"><span data-stu-id="b6368-141">CSV</span></span>

<span data-ttu-id="b6368-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b6368-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b6368-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6368-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b6368-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b6368-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b6368-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b6368-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b6368-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b6368-146">Report Refresh Date</span></span>
- <span data-ttu-id="b6368-147">Enviar</span><span class="sxs-lookup"><span data-stu-id="b6368-147">Send</span></span>
- <span data-ttu-id="b6368-148">Receber</span><span class="sxs-lookup"><span data-stu-id="b6368-148">Receive</span></span>
- <span data-ttu-id="b6368-149">Ler</span><span class="sxs-lookup"><span data-stu-id="b6368-149">Read</span></span>
- <span data-ttu-id="b6368-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b6368-150">Report Date</span></span>
- <span data-ttu-id="b6368-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b6368-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b6368-152">JSON</span><span class="sxs-lookup"><span data-stu-id="b6368-152">JSON</span></span>

<span data-ttu-id="b6368-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[emailActivitySummary](../resources/emailactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6368-153">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6368-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6368-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b6368-155">CSV</span><span class="sxs-lookup"><span data-stu-id="b6368-155">CSV</span></span>

<span data-ttu-id="b6368-156">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="b6368-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b6368-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6368-157">Request</span></span>

<span data-ttu-id="b6368-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6368-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b6368-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6368-159">Response</span></span>

<span data-ttu-id="b6368-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6368-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b6368-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b6368-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b6368-162">JSON</span><span class="sxs-lookup"><span data-stu-id="b6368-162">JSON</span></span>

<span data-ttu-id="b6368-163">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="b6368-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b6368-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6368-164">Request</span></span>

<span data-ttu-id="b6368-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6368-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b6368-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6368-166">Response</span></span>

<span data-ttu-id="b6368-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6368-167">The following is an example of the response.</span></span>

> <span data-ttu-id="b6368-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6368-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 504, 
      "receive": 76506, 
      "read": 12161, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
