---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6115368b99c1aa8c445e9d6f7e7c307a4b72f8e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336326"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="67ceb-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="67ceb-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67ceb-105">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="67ceb-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="67ceb-106">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="67ceb-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="67ceb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="67ceb-107">Permissions</span></span>

<span data-ttu-id="67ceb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67ceb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67ceb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67ceb-110">Permission type</span></span>                        | <span data-ttu-id="67ceb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67ceb-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="67ceb-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67ceb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="67ceb-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67ceb-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="67ceb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67ceb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ceb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67ceb-115">Not supported.</span></span>                           |
| <span data-ttu-id="67ceb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67ceb-116">Application</span></span>                            | <span data-ttu-id="67ceb-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67ceb-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="67ceb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67ceb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="67ceb-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="67ceb-119">Function parameters</span></span>

<span data-ttu-id="67ceb-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="67ceb-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="67ceb-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="67ceb-121">Parameter</span></span> | <span data-ttu-id="67ceb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="67ceb-122">Type</span></span>   | <span data-ttu-id="67ceb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ceb-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="67ceb-124">ponto</span><span class="sxs-lookup"><span data-stu-id="67ceb-124">period</span></span>    | <span data-ttu-id="67ceb-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67ceb-125">string</span></span> | <span data-ttu-id="67ceb-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="67ceb-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="67ceb-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="67ceb-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="67ceb-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="67ceb-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="67ceb-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67ceb-129">Required.</span></span> |

<span data-ttu-id="67ceb-130">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67ceb-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="67ceb-131">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="67ceb-131">The default output type is text/csv.</span></span> <span data-ttu-id="67ceb-132">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="67ceb-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67ceb-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67ceb-133">Request headers</span></span>

| <span data-ttu-id="67ceb-134">Nome</span><span class="sxs-lookup"><span data-stu-id="67ceb-134">Name</span></span>          | <span data-ttu-id="67ceb-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ceb-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="67ceb-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="67ceb-136">Authorization</span></span> | <span data-ttu-id="67ceb-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67ceb-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="67ceb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ceb-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="67ceb-140">CSV</span><span class="sxs-lookup"><span data-stu-id="67ceb-140">CSV</span></span>

<span data-ttu-id="67ceb-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="67ceb-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="67ceb-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="67ceb-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="67ceb-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="67ceb-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="67ceb-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="67ceb-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="67ceb-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="67ceb-145">Report Refresh Date</span></span>
- <span data-ttu-id="67ceb-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="67ceb-146">Report Date</span></span>
- <span data-ttu-id="67ceb-147">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="67ceb-147">Team Chat Messages</span></span>
- <span data-ttu-id="67ceb-148">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="67ceb-148">Private Chat Messages</span></span>
- <span data-ttu-id="67ceb-149">Chamadas</span><span class="sxs-lookup"><span data-stu-id="67ceb-149">Calls</span></span>
- <span data-ttu-id="67ceb-150">Reuniões</span><span class="sxs-lookup"><span data-stu-id="67ceb-150">Meetings</span></span>
- <span data-ttu-id="67ceb-151">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="67ceb-151">Other Actions</span></span>
- <span data-ttu-id="67ceb-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="67ceb-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="67ceb-153">JSON</span><span class="sxs-lookup"><span data-stu-id="67ceb-153">JSON</span></span>

<span data-ttu-id="67ceb-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67ceb-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67ceb-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67ceb-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="67ceb-156">CSV</span><span class="sxs-lookup"><span data-stu-id="67ceb-156">CSV</span></span>

<span data-ttu-id="67ceb-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="67ceb-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="67ceb-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67ceb-158">Request</span></span>

<span data-ttu-id="67ceb-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67ceb-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="67ceb-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ceb-160">Response</span></span>

<span data-ttu-id="67ceb-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67ceb-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="67ceb-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="67ceb-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="67ceb-163">JSON</span><span class="sxs-lookup"><span data-stu-id="67ceb-163">JSON</span></span>

<span data-ttu-id="67ceb-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="67ceb-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="67ceb-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67ceb-165">Request</span></span>

<span data-ttu-id="67ceb-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67ceb-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="67ceb-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ceb-167">Response</span></span>

<span data-ttu-id="67ceb-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67ceb-168">The following is an example of the response.</span></span>

> <span data-ttu-id="67ceb-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67ceb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
