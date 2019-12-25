---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 21f311cb86237ecfd35997ff3950ee9bc86f22d6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867537"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="de9df-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="de9df-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de9df-104">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="de9df-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="de9df-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="de9df-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="de9df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de9df-106">Permissions</span></span>

<span data-ttu-id="de9df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de9df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de9df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de9df-109">Permission type</span></span>                        | <span data-ttu-id="de9df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de9df-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="de9df-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de9df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de9df-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="de9df-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="de9df-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de9df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de9df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de9df-114">Not supported.</span></span>                           |
| <span data-ttu-id="de9df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de9df-115">Application</span></span>                            | <span data-ttu-id="de9df-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="de9df-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="de9df-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="de9df-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="de9df-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="de9df-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="de9df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de9df-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="de9df-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="de9df-120">Function parameters</span></span>

<span data-ttu-id="de9df-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="de9df-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="de9df-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="de9df-122">Parameter</span></span> | <span data-ttu-id="de9df-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="de9df-123">Type</span></span>   | <span data-ttu-id="de9df-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="de9df-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="de9df-125">ponto</span><span class="sxs-lookup"><span data-stu-id="de9df-125">period</span></span>    | <span data-ttu-id="de9df-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de9df-126">string</span></span> | <span data-ttu-id="de9df-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="de9df-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="de9df-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="de9df-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="de9df-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="de9df-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="de9df-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de9df-130">Required.</span></span> |

<span data-ttu-id="de9df-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de9df-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="de9df-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="de9df-132">The default output type is text/csv.</span></span> <span data-ttu-id="de9df-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="de9df-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de9df-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de9df-134">Request headers</span></span>

| <span data-ttu-id="de9df-135">Nome</span><span class="sxs-lookup"><span data-stu-id="de9df-135">Name</span></span>          | <span data-ttu-id="de9df-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="de9df-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="de9df-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="de9df-137">Authorization</span></span> | <span data-ttu-id="de9df-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de9df-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="de9df-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="de9df-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="de9df-141">CSV</span><span class="sxs-lookup"><span data-stu-id="de9df-141">CSV</span></span>

<span data-ttu-id="de9df-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="de9df-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="de9df-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="de9df-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="de9df-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="de9df-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="de9df-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="de9df-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="de9df-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="de9df-146">Report Refresh Date</span></span>
- <span data-ttu-id="de9df-147">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="de9df-147">Exchange Emails Received</span></span>
- <span data-ttu-id="de9df-148">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="de9df-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="de9df-149">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="de9df-149">Yammer Messages Read</span></span>
- <span data-ttu-id="de9df-150">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="de9df-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="de9df-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="de9df-151">Report Date</span></span>
- <span data-ttu-id="de9df-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="de9df-152">Report Period</span></span>

<span data-ttu-id="de9df-153">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="de9df-153">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="de9df-154">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="de9df-154">Yammer Messages Posted</span></span>
- <span data-ttu-id="de9df-155">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="de9df-155">Yammer Messages Read</span></span>
- <span data-ttu-id="de9df-156">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="de9df-156">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="de9df-157">JSON</span><span class="sxs-lookup"><span data-stu-id="de9df-157">JSON</span></span>

<span data-ttu-id="de9df-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de9df-158">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="de9df-159">As propriedades a seguir no objeto **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="de9df-159">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="de9df-160">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="de9df-160">yammerMessagesPosted</span></span>
- <span data-ttu-id="de9df-161">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="de9df-161">yammerMessagesRead</span></span>
- <span data-ttu-id="de9df-162">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="de9df-162">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="de9df-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de9df-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="de9df-164">CSV</span><span class="sxs-lookup"><span data-stu-id="de9df-164">CSV</span></span>

<span data-ttu-id="de9df-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="de9df-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="de9df-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de9df-166">Request</span></span>

<span data-ttu-id="de9df-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de9df-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de9df-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="de9df-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de9df-169">C#</span><span class="sxs-lookup"><span data-stu-id="de9df-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de9df-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de9df-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de9df-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de9df-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="de9df-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="de9df-172">Response</span></span>

<span data-ttu-id="de9df-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de9df-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="de9df-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="de9df-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="de9df-175">JSON</span><span class="sxs-lookup"><span data-stu-id="de9df-175">JSON</span></span>

<span data-ttu-id="de9df-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="de9df-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="de9df-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de9df-177">Request</span></span>

<span data-ttu-id="de9df-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de9df-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de9df-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="de9df-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de9df-180">C#</span><span class="sxs-lookup"><span data-stu-id="de9df-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de9df-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de9df-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de9df-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de9df-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="de9df-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="de9df-183">Response</span></span>

<span data-ttu-id="de9df-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de9df-184">The following is an example of the response.</span></span>

> <span data-ttu-id="de9df-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de9df-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
