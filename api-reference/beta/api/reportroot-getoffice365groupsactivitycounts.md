---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4ebc05ac2b990f50628c028e157cbb50681f5f4e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336786"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="9bf2b-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="9bf2b-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bf2b-104">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="9bf2b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="9bf2b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="9bf2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bf2b-106">Permissions</span></span>

<span data-ttu-id="9bf2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9bf2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bf2b-109">Permission type</span></span>                        | <span data-ttu-id="9bf2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bf2b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9bf2b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bf2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9bf2b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bf2b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9bf2b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bf2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bf2b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-114">Not supported.</span></span>                           |
| <span data-ttu-id="9bf2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bf2b-115">Application</span></span>                            | <span data-ttu-id="9bf2b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bf2b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9bf2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf2b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9bf2b-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9bf2b-118">Function parameters</span></span>

<span data-ttu-id="9bf2b-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9bf2b-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9bf2b-120">Parameter</span></span> | <span data-ttu-id="9bf2b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf2b-121">Type</span></span>   | <span data-ttu-id="9bf2b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf2b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9bf2b-123">ponto</span><span class="sxs-lookup"><span data-stu-id="9bf2b-123">period</span></span>    | <span data-ttu-id="9bf2b-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf2b-124">string</span></span> | <span data-ttu-id="9bf2b-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9bf2b-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9bf2b-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9bf2b-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-128">Required.</span></span> |

<span data-ttu-id="9bf2b-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9bf2b-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-130">The default output type is text/csv.</span></span> <span data-ttu-id="9bf2b-131">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bf2b-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf2b-132">Request headers</span></span>

| <span data-ttu-id="9bf2b-133">Nome</span><span class="sxs-lookup"><span data-stu-id="9bf2b-133">Name</span></span>          | <span data-ttu-id="9bf2b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf2b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9bf2b-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bf2b-135">Authorization</span></span> | <span data-ttu-id="9bf2b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9bf2b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf2b-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9bf2b-139">CSV</span><span class="sxs-lookup"><span data-stu-id="9bf2b-139">CSV</span></span>

<span data-ttu-id="9bf2b-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9bf2b-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9bf2b-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9bf2b-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9bf2b-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9bf2b-144">Report Refresh Date</span></span>
- <span data-ttu-id="9bf2b-145">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="9bf2b-145">Exchange Emails Received</span></span>
- <span data-ttu-id="9bf2b-146">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="9bf2b-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="9bf2b-147">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="9bf2b-147">Yammer Messages Read</span></span>
- <span data-ttu-id="9bf2b-148">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="9bf2b-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="9bf2b-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="9bf2b-149">Report Date</span></span>
- <span data-ttu-id="9bf2b-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9bf2b-150">Report Period</span></span>

<span data-ttu-id="9bf2b-151">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="9bf2b-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9bf2b-152">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="9bf2b-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="9bf2b-153">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="9bf2b-153">Yammer Messages Read</span></span>
- <span data-ttu-id="9bf2b-154">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="9bf2b-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="9bf2b-155">JSON</span><span class="sxs-lookup"><span data-stu-id="9bf2b-155">JSON</span></span>

<span data-ttu-id="9bf2b-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="9bf2b-157">As propriedades a seguir no objeto **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="9bf2b-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9bf2b-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="9bf2b-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="9bf2b-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="9bf2b-159">yammerMessagesRead</span></span>
- <span data-ttu-id="9bf2b-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="9bf2b-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="9bf2b-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bf2b-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9bf2b-162">CSV</span><span class="sxs-lookup"><span data-stu-id="9bf2b-162">CSV</span></span>

<span data-ttu-id="9bf2b-163">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9bf2b-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf2b-164">Request</span></span>

<span data-ttu-id="9bf2b-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9bf2b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf2b-166">Response</span></span>

<span data-ttu-id="9bf2b-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9bf2b-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="9bf2b-169">JSON</span><span class="sxs-lookup"><span data-stu-id="9bf2b-169">JSON</span></span>

<span data-ttu-id="9bf2b-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9bf2b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf2b-171">Request</span></span>

<span data-ttu-id="9bf2b-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9bf2b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf2b-173">Response</span></span>

<span data-ttu-id="9bf2b-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-174">The following is an example of the response.</span></span>

> <span data-ttu-id="9bf2b-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bf2b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
