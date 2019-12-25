---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d7489fe5de57ef8d1b9b3a9f435670333de42f91
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867329"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="29fb3-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="29fb3-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29fb3-105">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="29fb3-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="29fb3-106">Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="29fb3-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="29fb3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29fb3-107">Permissions</span></span>

<span data-ttu-id="29fb3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29fb3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29fb3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29fb3-110">Permission type</span></span>                        | <span data-ttu-id="29fb3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29fb3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="29fb3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29fb3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="29fb3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29fb3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="29fb3-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29fb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29fb3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29fb3-115">Not supported.</span></span>                           |
| <span data-ttu-id="29fb3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29fb3-116">Application</span></span>                            | <span data-ttu-id="29fb3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29fb3-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="29fb3-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="29fb3-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="29fb3-119">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="29fb3-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="29fb3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29fb3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="29fb3-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="29fb3-121">Function parameters</span></span>

<span data-ttu-id="29fb3-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="29fb3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="29fb3-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="29fb3-123">Parameter</span></span> | <span data-ttu-id="29fb3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="29fb3-124">Type</span></span>   | <span data-ttu-id="29fb3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fb3-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="29fb3-126">ponto</span><span class="sxs-lookup"><span data-stu-id="29fb3-126">period</span></span>    | <span data-ttu-id="29fb3-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29fb3-127">string</span></span> | <span data-ttu-id="29fb3-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="29fb3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="29fb3-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="29fb3-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="29fb3-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="29fb3-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="29fb3-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29fb3-131">Required.</span></span> |

<span data-ttu-id="29fb3-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29fb3-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="29fb3-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="29fb3-133">The default output type is text/csv.</span></span> <span data-ttu-id="29fb3-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="29fb3-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29fb3-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29fb3-135">Request headers</span></span>

| <span data-ttu-id="29fb3-136">Nome</span><span class="sxs-lookup"><span data-stu-id="29fb3-136">Name</span></span>          | <span data-ttu-id="29fb3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fb3-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="29fb3-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="29fb3-138">Authorization</span></span> | <span data-ttu-id="29fb3-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29fb3-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="29fb3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fb3-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="29fb3-142">CSV</span><span class="sxs-lookup"><span data-stu-id="29fb3-142">CSV</span></span>

<span data-ttu-id="29fb3-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="29fb3-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="29fb3-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="29fb3-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="29fb3-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="29fb3-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="29fb3-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="29fb3-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="29fb3-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="29fb3-147">Report Refresh Date</span></span>
- <span data-ttu-id="29fb3-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="29fb3-148">Report Date</span></span>
- <span data-ttu-id="29fb3-149">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="29fb3-149">Team Chat Messages</span></span>
- <span data-ttu-id="29fb3-150">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="29fb3-150">Private Chat Messages</span></span>
- <span data-ttu-id="29fb3-151">Chamadas</span><span class="sxs-lookup"><span data-stu-id="29fb3-151">Calls</span></span>
- <span data-ttu-id="29fb3-152">Reuniões</span><span class="sxs-lookup"><span data-stu-id="29fb3-152">Meetings</span></span>
- <span data-ttu-id="29fb3-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="29fb3-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="29fb3-154">JSON</span><span class="sxs-lookup"><span data-stu-id="29fb3-154">JSON</span></span>

<span data-ttu-id="29fb3-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29fb3-155">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29fb3-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29fb3-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="29fb3-157">CSV</span><span class="sxs-lookup"><span data-stu-id="29fb3-157">CSV</span></span>

<span data-ttu-id="29fb3-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="29fb3-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="29fb3-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29fb3-159">Request</span></span>

<span data-ttu-id="29fb3-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29fb3-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="29fb3-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="29fb3-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29fb3-162">C#</span><span class="sxs-lookup"><span data-stu-id="29fb3-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29fb3-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29fb3-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29fb3-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29fb3-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29fb3-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fb3-165">Response</span></span>

<span data-ttu-id="29fb3-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29fb3-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="29fb3-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="29fb3-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="29fb3-168">JSON</span><span class="sxs-lookup"><span data-stu-id="29fb3-168">JSON</span></span>

<span data-ttu-id="29fb3-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="29fb3-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="29fb3-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29fb3-170">Request</span></span>

<span data-ttu-id="29fb3-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29fb3-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="29fb3-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="29fb3-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29fb3-173">C#</span><span class="sxs-lookup"><span data-stu-id="29fb3-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29fb3-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29fb3-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29fb3-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29fb3-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29fb3-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fb3-176">Response</span></span>

<span data-ttu-id="29fb3-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29fb3-177">The following is an example of the response.</span></span>

> <span data-ttu-id="29fb3-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29fb3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
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
