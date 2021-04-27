---
title: 'reportRoot: getTeamsUserActivityDistributionUserCounts'
description: Obter o número de usuários Microsoft Teams licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 69bdcafd963c96274034f53158337d0e38c3d654
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053514"
---
# <a name="reportroot-getteamsuseractivitydistributionusercounts"></a><span data-ttu-id="47867-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="47867-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span></span>

<span data-ttu-id="47867-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47867-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47867-106">Obter o número de usuários Microsoft Teams licenciados por tipo de atividade durante o período selecionado.</span><span class="sxs-lookup"><span data-stu-id="47867-106">Get the number of Microsoft Teams licensed users by activity type over the selected period.</span></span> <span data-ttu-id="47867-107">Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="47867-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="47867-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="47867-108">Permissions</span></span>

<span data-ttu-id="47867-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47867-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47867-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47867-111">Permission type</span></span>                        | <span data-ttu-id="47867-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47867-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="47867-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47867-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="47867-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47867-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="47867-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47867-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47867-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47867-116">Not supported.</span></span>                           |
| <span data-ttu-id="47867-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47867-117">Application</span></span>                            | <span data-ttu-id="47867-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47867-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="47867-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="47867-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="47867-120">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="47867-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="47867-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47867-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="47867-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="47867-122">Function parameters</span></span>

<span data-ttu-id="47867-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="47867-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="47867-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47867-124">Parameter</span></span> | <span data-ttu-id="47867-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="47867-125">Type</span></span>   | <span data-ttu-id="47867-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="47867-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="47867-127">ponto</span><span class="sxs-lookup"><span data-stu-id="47867-127">period</span></span>    | <span data-ttu-id="47867-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47867-128">string</span></span> | <span data-ttu-id="47867-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="47867-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="47867-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="47867-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="47867-131">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="47867-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="47867-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47867-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="47867-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47867-133">Optional query parameters</span></span>

<span data-ttu-id="47867-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47867-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="47867-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="47867-135">The default output type is text/csv.</span></span> <span data-ttu-id="47867-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData definido como `$format` text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="47867-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47867-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47867-137">Request headers</span></span>

| <span data-ttu-id="47867-138">Nome</span><span class="sxs-lookup"><span data-stu-id="47867-138">Name</span></span>          | <span data-ttu-id="47867-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="47867-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="47867-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="47867-140">Authorization</span></span> | <span data-ttu-id="47867-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47867-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="47867-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="47867-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="47867-144">CSV</span><span class="sxs-lookup"><span data-stu-id="47867-144">CSV</span></span>

<span data-ttu-id="47867-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="47867-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="47867-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="47867-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="47867-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="47867-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="47867-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="47867-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="47867-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="47867-149">Report Refresh Date</span></span>
- <span data-ttu-id="47867-150">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="47867-150">Team Chat Messages</span></span>
- <span data-ttu-id="47867-151">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="47867-151">Private Chat Messages</span></span>
- <span data-ttu-id="47867-152">Chamadas</span><span class="sxs-lookup"><span data-stu-id="47867-152">Calls</span></span>
- <span data-ttu-id="47867-153">Reuniões</span><span class="sxs-lookup"><span data-stu-id="47867-153">Meetings</span></span>
- <span data-ttu-id="47867-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="47867-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="47867-155">JSON</span><span class="sxs-lookup"><span data-stu-id="47867-155">JSON</span></span>

<span data-ttu-id="47867-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47867-156">If successful, this method returns a `200 OK` response code and a [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47867-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47867-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="47867-158">CSV</span><span class="sxs-lookup"><span data-stu-id="47867-158">CSV</span></span>

<span data-ttu-id="47867-159">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="47867-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="47867-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47867-160">Request</span></span>

<span data-ttu-id="47867-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47867-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="47867-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="47867-162">Response</span></span>

<span data-ttu-id="47867-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47867-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="47867-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="47867-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="47867-165">JSON</span><span class="sxs-lookup"><span data-stu-id="47867-165">JSON</span></span>

<span data-ttu-id="47867-166">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="47867-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="47867-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47867-167">Request</span></span>

<span data-ttu-id="47867-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47867-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="47867-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="47867-169">Response</span></span>

<span data-ttu-id="47867-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47867-170">The following is an example of the response.</span></span>

> <span data-ttu-id="47867-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47867-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsuseractivitydistributionusercounts)", 
  "value": [
    {
      "reportRefreshDate": "2020-09-01", 
      "teamChatMessages": 0, 
      "privateChatMessages": 0, 
      "calls": 0, 
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


