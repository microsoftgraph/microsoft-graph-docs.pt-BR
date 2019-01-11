---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.openlocfilehash: 4ee6dc35f93188b63d5c3ab4b6a7733e015747f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841066"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="44a43-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="44a43-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

> <span data-ttu-id="44a43-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="44a43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44a43-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="44a43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44a43-106">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="44a43-106">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="44a43-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="44a43-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="44a43-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="44a43-108">Permissions</span></span>

<span data-ttu-id="44a43-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44a43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44a43-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44a43-111">Permission type</span></span>                        | <span data-ttu-id="44a43-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44a43-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44a43-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44a43-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="44a43-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a43-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44a43-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44a43-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44a43-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44a43-116">Not supported.</span></span>                           |
| <span data-ttu-id="44a43-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44a43-117">Application</span></span>                            | <span data-ttu-id="44a43-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a43-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="44a43-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44a43-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="44a43-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="44a43-120">Function parameters</span></span>

<span data-ttu-id="44a43-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="44a43-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="44a43-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="44a43-122">Parameter</span></span> | <span data-ttu-id="44a43-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="44a43-123">Type</span></span>   | <span data-ttu-id="44a43-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="44a43-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44a43-125">ponto</span><span class="sxs-lookup"><span data-stu-id="44a43-125">period</span></span>    | <span data-ttu-id="44a43-126">string</span><span class="sxs-lookup"><span data-stu-id="44a43-126">string</span></span> | <span data-ttu-id="44a43-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="44a43-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44a43-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="44a43-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44a43-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="44a43-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="44a43-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44a43-130">Required.</span></span> |

<span data-ttu-id="44a43-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44a43-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="44a43-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="44a43-132">The default output type is text/csv.</span></span> <span data-ttu-id="44a43-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="44a43-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44a43-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44a43-134">Request headers</span></span>

| <span data-ttu-id="44a43-135">Nome</span><span class="sxs-lookup"><span data-stu-id="44a43-135">Name</span></span>          | <span data-ttu-id="44a43-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="44a43-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="44a43-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="44a43-137">Authorization</span></span> | <span data-ttu-id="44a43-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44a43-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="44a43-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="44a43-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="44a43-141">CSV</span><span class="sxs-lookup"><span data-stu-id="44a43-141">CSV</span></span>

<span data-ttu-id="44a43-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="44a43-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44a43-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="44a43-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44a43-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="44a43-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44a43-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="44a43-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="44a43-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="44a43-146">Report Refresh Date</span></span>
- <span data-ttu-id="44a43-147">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="44a43-147">Exchange Emails Received</span></span>
- <span data-ttu-id="44a43-148">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="44a43-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="44a43-149">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="44a43-149">Yammer Messages Read</span></span>
- <span data-ttu-id="44a43-150">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="44a43-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="44a43-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="44a43-151">Report Date</span></span>
- <span data-ttu-id="44a43-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="44a43-152">Report Period</span></span>

<span data-ttu-id="44a43-153">Não há suporte para as seguintes colunas na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="44a43-153">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="44a43-154">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="44a43-154">Yammer Messages Posted</span></span>
- <span data-ttu-id="44a43-155">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="44a43-155">Yammer Messages Read</span></span>
- <span data-ttu-id="44a43-156">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="44a43-156">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="44a43-157">JSON</span><span class="sxs-lookup"><span data-stu-id="44a43-157">JSON</span></span>

<span data-ttu-id="44a43-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44a43-158">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="44a43-159">Não há suporte para as seguintes propriedades no objeto **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="44a43-159">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="44a43-160">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="44a43-160">yammerMessagesPosted</span></span>
- <span data-ttu-id="44a43-161">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="44a43-161">yammerMessagesRead</span></span>
- <span data-ttu-id="44a43-162">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="44a43-162">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="44a43-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44a43-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="44a43-164">CSV</span><span class="sxs-lookup"><span data-stu-id="44a43-164">CSV</span></span>

<span data-ttu-id="44a43-165">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="44a43-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="44a43-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44a43-166">Request</span></span>

<span data-ttu-id="44a43-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44a43-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="44a43-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="44a43-168">Response</span></span>

<span data-ttu-id="44a43-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44a43-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="44a43-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="44a43-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="44a43-171">JSON</span><span class="sxs-lookup"><span data-stu-id="44a43-171">JSON</span></span>

<span data-ttu-id="44a43-172">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="44a43-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="44a43-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44a43-173">Request</span></span>

<span data-ttu-id="44a43-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44a43-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="44a43-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="44a43-175">Response</span></span>

<span data-ttu-id="44a43-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44a43-176">The following is an example of the response.</span></span>

> <span data-ttu-id="44a43-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44a43-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
