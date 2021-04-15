---
title: 'reportRoot: getTeamsUserActivityTotalUserCounts'
description: Obter o número de usuários licenciados ou não licenciados do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9c62a7bf316f8b11b908f30eb3db1865b7a4f1df
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766903"
---
# <a name="reportroot-getteamsuseractivitytotalusercounts"></a><span data-ttu-id="7ca2f-104">reportRoot: getTeamsUserActivityTotalUserCounts</span><span class="sxs-lookup"><span data-stu-id="7ca2f-104">reportRoot: getTeamsUserActivityTotalUserCounts</span></span>

<span data-ttu-id="7ca2f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca2f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ca2f-106">Obter o número de usuários licenciados ou não licenciados do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-106">Get the number of Microsoft Teams licensed or non-licensed users by activity type.</span></span> <span data-ttu-id="7ca2f-107">Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ca2f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ca2f-108">Permissions</span></span>

<span data-ttu-id="7ca2f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ca2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ca2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ca2f-111">Permission type</span></span>                        | <span data-ttu-id="7ca2f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ca2f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7ca2f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ca2f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ca2f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ca2f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7ca2f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ca2f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ca2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-116">Not supported.</span></span>                           |
| <span data-ttu-id="7ca2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ca2f-117">Application</span></span>                            | <span data-ttu-id="7ca2f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ca2f-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="7ca2f-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7ca2f-120">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7ca2f-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7ca2f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ca2f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="7ca2f-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7ca2f-122">Function parameters</span></span>

<span data-ttu-id="7ca2f-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7ca2f-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7ca2f-124">Parameter</span></span> | <span data-ttu-id="7ca2f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ca2f-125">Type</span></span>   | <span data-ttu-id="7ca2f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ca2f-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7ca2f-127">ponto</span><span class="sxs-lookup"><span data-stu-id="7ca2f-127">period</span></span>    | <span data-ttu-id="7ca2f-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ca2f-128">string</span></span> | <span data-ttu-id="7ca2f-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7ca2f-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7ca2f-131">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7ca2f-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="7ca2f-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ca2f-133">Optional query parameters</span></span>

<span data-ttu-id="7ca2f-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7ca2f-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-135">The default output type is text/csv.</span></span> <span data-ttu-id="7ca2f-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData definido como `$format` text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ca2f-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ca2f-137">Request headers</span></span>

| <span data-ttu-id="7ca2f-138">Nome</span><span class="sxs-lookup"><span data-stu-id="7ca2f-138">Name</span></span>          | <span data-ttu-id="7ca2f-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ca2f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7ca2f-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ca2f-140">Authorization</span></span> | <span data-ttu-id="7ca2f-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7ca2f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ca2f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7ca2f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="7ca2f-144">CSV</span></span>

<span data-ttu-id="7ca2f-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7ca2f-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7ca2f-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7ca2f-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7ca2f-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7ca2f-149">Report Refresh Date</span></span>
- <span data-ttu-id="7ca2f-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="7ca2f-150">Report Date</span></span>
- <span data-ttu-id="7ca2f-151">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="7ca2f-151">Team Chat Messages</span></span>
- <span data-ttu-id="7ca2f-152">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="7ca2f-152">Private Chat Messages</span></span>
- <span data-ttu-id="7ca2f-153">Chamadas</span><span class="sxs-lookup"><span data-stu-id="7ca2f-153">Calls</span></span>
- <span data-ttu-id="7ca2f-154">Reuniões</span><span class="sxs-lookup"><span data-stu-id="7ca2f-154">Meetings</span></span>
- <span data-ttu-id="7ca2f-155">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="7ca2f-155">Other Actions</span></span>
- <span data-ttu-id="7ca2f-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7ca2f-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7ca2f-157">JSON</span><span class="sxs-lookup"><span data-stu-id="7ca2f-157">JSON</span></span>

<span data-ttu-id="7ca2f-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-158">If successful, this method returns a `200 OK` response code and a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ca2f-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ca2f-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7ca2f-160">CSV</span><span class="sxs-lookup"><span data-stu-id="7ca2f-160">CSV</span></span>

<span data-ttu-id="7ca2f-161">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7ca2f-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ca2f-162">Request</span></span>

<span data-ttu-id="7ca2f-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7ca2f-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ca2f-164">Response</span></span>

<span data-ttu-id="7ca2f-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7ca2f-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7ca2f-167">JSON</span><span class="sxs-lookup"><span data-stu-id="7ca2f-167">JSON</span></span>

<span data-ttu-id="7ca2f-168">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7ca2f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ca2f-169">Request</span></span>

<span data-ttu-id="7ca2f-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7ca2f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ca2f-171">Response</span></span>

<span data-ttu-id="7ca2f-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-172">The following is an example of the response.</span></span>

> <span data-ttu-id="7ca2f-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ca2f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
