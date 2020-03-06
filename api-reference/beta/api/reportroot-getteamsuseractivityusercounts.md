---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3184bdaa59f5203f3d3f3630ed8477de55c91d44
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454021"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="3a748-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="3a748-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="3a748-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a748-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a748-106">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="3a748-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="3a748-107">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="3a748-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a748-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a748-108">Permissions</span></span>

<span data-ttu-id="3a748-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a748-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a748-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a748-111">Permission type</span></span>                        | <span data-ttu-id="3a748-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a748-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3a748-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a748-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a748-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a748-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3a748-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a748-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a748-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a748-116">Not supported.</span></span>                           |
| <span data-ttu-id="3a748-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a748-117">Application</span></span>                            | <span data-ttu-id="3a748-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a748-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="3a748-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3a748-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3a748-120">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3a748-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3a748-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a748-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="3a748-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3a748-122">Function parameters</span></span>

<span data-ttu-id="3a748-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3a748-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3a748-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a748-124">Parameter</span></span> | <span data-ttu-id="3a748-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a748-125">Type</span></span>   | <span data-ttu-id="3a748-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a748-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3a748-127">ponto</span><span class="sxs-lookup"><span data-stu-id="3a748-127">period</span></span>    | <span data-ttu-id="3a748-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a748-128">string</span></span> | <span data-ttu-id="3a748-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3a748-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3a748-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3a748-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3a748-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3a748-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3a748-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a748-132">Required.</span></span> |

<span data-ttu-id="3a748-133">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a748-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3a748-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="3a748-134">The default output type is text/csv.</span></span> <span data-ttu-id="3a748-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="3a748-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a748-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a748-136">Request headers</span></span>

| <span data-ttu-id="3a748-137">Nome</span><span class="sxs-lookup"><span data-stu-id="3a748-137">Name</span></span>          | <span data-ttu-id="3a748-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a748-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3a748-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a748-139">Authorization</span></span> | <span data-ttu-id="3a748-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a748-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3a748-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a748-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3a748-143">CSV</span><span class="sxs-lookup"><span data-stu-id="3a748-143">CSV</span></span>

<span data-ttu-id="3a748-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3a748-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3a748-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3a748-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3a748-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3a748-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3a748-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3a748-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3a748-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3a748-148">Report Refresh Date</span></span>
- <span data-ttu-id="3a748-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3a748-149">Report Date</span></span>
- <span data-ttu-id="3a748-150">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="3a748-150">Team Chat Messages</span></span>
- <span data-ttu-id="3a748-151">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="3a748-151">Private Chat Messages</span></span>
- <span data-ttu-id="3a748-152">Chamadas</span><span class="sxs-lookup"><span data-stu-id="3a748-152">Calls</span></span>
- <span data-ttu-id="3a748-153">Reuniões</span><span class="sxs-lookup"><span data-stu-id="3a748-153">Meetings</span></span>
- <span data-ttu-id="3a748-154">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="3a748-154">Other Actions</span></span>
- <span data-ttu-id="3a748-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3a748-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3a748-156">JSON</span><span class="sxs-lookup"><span data-stu-id="3a748-156">JSON</span></span>

<span data-ttu-id="3a748-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a748-157">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a748-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a748-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3a748-159">CSV</span><span class="sxs-lookup"><span data-stu-id="3a748-159">CSV</span></span>

<span data-ttu-id="3a748-160">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="3a748-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3a748-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a748-161">Request</span></span>

<span data-ttu-id="3a748-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a748-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a748-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a748-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="3a748-164">C#</span><span class="sxs-lookup"><span data-stu-id="3a748-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a748-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a748-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a748-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a748-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a748-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a748-167">Response</span></span>

<span data-ttu-id="3a748-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a748-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3a748-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3a748-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3a748-170">JSON</span><span class="sxs-lookup"><span data-stu-id="3a748-170">JSON</span></span>

<span data-ttu-id="3a748-171">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="3a748-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3a748-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a748-172">Request</span></span>

<span data-ttu-id="3a748-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a748-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a748-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a748-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="3a748-175">C#</span><span class="sxs-lookup"><span data-stu-id="3a748-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a748-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a748-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a748-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a748-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a748-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a748-178">Response</span></span>

<span data-ttu-id="3a748-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a748-179">The following is an example of the response.</span></span>

> <span data-ttu-id="3a748-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a748-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
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
