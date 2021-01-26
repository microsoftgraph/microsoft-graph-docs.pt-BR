---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: c4ded882d6a90755ec25e6635d5949fd8b846b6a
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983080"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="4c683-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4c683-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="4c683-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c683-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c683-105">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="4c683-105">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="4c683-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - grupos do Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="4c683-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c683-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c683-107">Permissions</span></span>

<span data-ttu-id="4c683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c683-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c683-110">Permission type</span></span>                        | <span data-ttu-id="4c683-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c683-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c683-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c683-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c683-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c683-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c683-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c683-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c683-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c683-115">Not supported.</span></span>                           |
| <span data-ttu-id="4c683-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c683-116">Application</span></span>                            | <span data-ttu-id="4c683-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c683-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="4c683-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="4c683-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4c683-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4c683-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4c683-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c683-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c683-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4c683-121">Function parameters</span></span>

<span data-ttu-id="4c683-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4c683-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c683-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4c683-123">Parameter</span></span> | <span data-ttu-id="4c683-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c683-124">Type</span></span>   | <span data-ttu-id="4c683-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c683-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c683-126">ponto</span><span class="sxs-lookup"><span data-stu-id="4c683-126">period</span></span>    | <span data-ttu-id="4c683-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c683-127">string</span></span> | <span data-ttu-id="4c683-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c683-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c683-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4c683-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c683-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c683-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c683-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c683-131">Required.</span></span> |

<span data-ttu-id="4c683-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c683-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c683-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="4c683-133">The default output type is text/csv.</span></span> <span data-ttu-id="4c683-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="4c683-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c683-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c683-135">Request headers</span></span>

| <span data-ttu-id="4c683-136">Nome</span><span class="sxs-lookup"><span data-stu-id="4c683-136">Name</span></span>          | <span data-ttu-id="4c683-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c683-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c683-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c683-138">Authorization</span></span> | <span data-ttu-id="4c683-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c683-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c683-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c683-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c683-142">CSV</span><span class="sxs-lookup"><span data-stu-id="4c683-142">CSV</span></span>

<span data-ttu-id="4c683-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4c683-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c683-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4c683-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c683-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c683-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c683-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4c683-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c683-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4c683-147">Report Refresh Date</span></span>
- <span data-ttu-id="4c683-148">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="4c683-148">Exchange Emails Received</span></span>
- <span data-ttu-id="4c683-149">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c683-149">Yammer Messages Posted</span></span>
- <span data-ttu-id="4c683-150">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c683-150">Yammer Messages Read</span></span>
- <span data-ttu-id="4c683-151">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c683-151">Yammer Messages Liked</span></span>
- <span data-ttu-id="4c683-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4c683-152">Report Date</span></span>
- <span data-ttu-id="4c683-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4c683-153">Report Period</span></span>

<span data-ttu-id="4c683-154">As seguintes colunas não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="4c683-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="4c683-155">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c683-155">Yammer Messages Posted</span></span>
- <span data-ttu-id="4c683-156">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c683-156">Yammer Messages Read</span></span>
- <span data-ttu-id="4c683-157">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c683-157">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="4c683-158">JSON</span><span class="sxs-lookup"><span data-stu-id="4c683-158">JSON</span></span>

<span data-ttu-id="4c683-159">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c683-159">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="4c683-160">As seguintes propriedades no **[objeto office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="4c683-160">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="4c683-161">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="4c683-161">yammerMessagesPosted</span></span>
- <span data-ttu-id="4c683-162">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="4c683-162">yammerMessagesRead</span></span>
- <span data-ttu-id="4c683-163">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="4c683-163">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="4c683-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c683-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c683-165">CSV</span><span class="sxs-lookup"><span data-stu-id="4c683-165">CSV</span></span>

<span data-ttu-id="4c683-166">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="4c683-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c683-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c683-167">Request</span></span>

<span data-ttu-id="4c683-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c683-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="4c683-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c683-169">Response</span></span>

<span data-ttu-id="4c683-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c683-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c683-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4c683-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4c683-172">JSON</span><span class="sxs-lookup"><span data-stu-id="4c683-172">JSON</span></span>

<span data-ttu-id="4c683-173">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="4c683-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c683-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c683-174">Request</span></span>

<span data-ttu-id="4c683-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c683-175">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="4c683-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c683-176">Response</span></span>

<span data-ttu-id="4c683-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c683-177">The following is an example of the response.</span></span>

> <span data-ttu-id="4c683-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c683-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


