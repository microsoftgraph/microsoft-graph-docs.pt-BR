---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões. As atividades são executadas por usuários licenciados do Microsoft Teams.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 8ac375460208e9f9f44d947ad4b764b82c390973
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766151"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="27aa2-105">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="27aa2-105">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="27aa2-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27aa2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27aa2-107">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="27aa2-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="27aa2-108">Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="27aa2-108">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span> <span data-ttu-id="27aa2-109">As atividades são executadas por usuários licenciados do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="27aa2-109">The activities are performed by Microsoft Teams licensed users.</span></span>

## <a name="permissions"></a><span data-ttu-id="27aa2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="27aa2-110">Permissions</span></span>

<span data-ttu-id="27aa2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27aa2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27aa2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27aa2-113">Permission type</span></span>                        | <span data-ttu-id="27aa2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27aa2-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="27aa2-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27aa2-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="27aa2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27aa2-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="27aa2-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27aa2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27aa2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27aa2-118">Not supported.</span></span>                           |
| <span data-ttu-id="27aa2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27aa2-119">Application</span></span>                            | <span data-ttu-id="27aa2-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27aa2-120">Reports.Read.All</span></span>                         |

<span data-ttu-id="27aa2-121">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="27aa2-121">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="27aa2-122">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="27aa2-122">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="27aa2-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27aa2-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="27aa2-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="27aa2-124">Function parameters</span></span>

<span data-ttu-id="27aa2-125">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="27aa2-125">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="27aa2-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27aa2-126">Parameter</span></span> | <span data-ttu-id="27aa2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="27aa2-127">Type</span></span>   | <span data-ttu-id="27aa2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="27aa2-128">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="27aa2-129">ponto</span><span class="sxs-lookup"><span data-stu-id="27aa2-129">period</span></span>    | <span data-ttu-id="27aa2-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27aa2-130">string</span></span> | <span data-ttu-id="27aa2-131">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="27aa2-131">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="27aa2-132">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="27aa2-132">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="27aa2-133">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="27aa2-133">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="27aa2-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27aa2-134">Required.</span></span> |

<span data-ttu-id="27aa2-135">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa2-135">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="27aa2-136">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="27aa2-136">The default output type is text/csv.</span></span> <span data-ttu-id="27aa2-137">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="27aa2-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27aa2-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa2-138">Request headers</span></span>

| <span data-ttu-id="27aa2-139">Nome</span><span class="sxs-lookup"><span data-stu-id="27aa2-139">Name</span></span>          | <span data-ttu-id="27aa2-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="27aa2-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="27aa2-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="27aa2-141">Authorization</span></span> | <span data-ttu-id="27aa2-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27aa2-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="27aa2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa2-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="27aa2-145">CSV</span><span class="sxs-lookup"><span data-stu-id="27aa2-145">CSV</span></span>

<span data-ttu-id="27aa2-146">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="27aa2-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="27aa2-147">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa2-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="27aa2-148">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="27aa2-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="27aa2-149">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="27aa2-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="27aa2-150">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="27aa2-150">Report Refresh Date</span></span>
- <span data-ttu-id="27aa2-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="27aa2-151">Report Date</span></span>
- <span data-ttu-id="27aa2-152">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="27aa2-152">Team Chat Messages</span></span>
- <span data-ttu-id="27aa2-153">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="27aa2-153">Private Chat Messages</span></span>
- <span data-ttu-id="27aa2-154">Chamadas</span><span class="sxs-lookup"><span data-stu-id="27aa2-154">Calls</span></span>
- <span data-ttu-id="27aa2-155">Reuniões</span><span class="sxs-lookup"><span data-stu-id="27aa2-155">Meetings</span></span>
- <span data-ttu-id="27aa2-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="27aa2-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="27aa2-157">JSON</span><span class="sxs-lookup"><span data-stu-id="27aa2-157">JSON</span></span>

<span data-ttu-id="27aa2-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa2-158">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27aa2-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27aa2-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="27aa2-160">CSV</span><span class="sxs-lookup"><span data-stu-id="27aa2-160">CSV</span></span>

<span data-ttu-id="27aa2-161">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="27aa2-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="27aa2-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa2-162">Request</span></span>

<span data-ttu-id="27aa2-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27aa2-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="27aa2-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa2-164">Response</span></span>

<span data-ttu-id="27aa2-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa2-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="27aa2-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="27aa2-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="27aa2-167">JSON</span><span class="sxs-lookup"><span data-stu-id="27aa2-167">JSON</span></span>

<span data-ttu-id="27aa2-168">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="27aa2-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="27aa2-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27aa2-169">Request</span></span>

<span data-ttu-id="27aa2-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27aa2-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="27aa2-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="27aa2-171">Response</span></span>

<span data-ttu-id="27aa2-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27aa2-172">The following is an example of the response.</span></span>

> <span data-ttu-id="27aa2-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27aa2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


