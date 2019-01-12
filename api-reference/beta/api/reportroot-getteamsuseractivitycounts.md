---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 614a8cc5f6e52b770d905c439cc9441cce7c6494
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982446"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="4949b-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4949b-104">reportRoot: getTeamsUserActivityCounts</span></span>

> <span data-ttu-id="4949b-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4949b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4949b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4949b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4949b-107">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="4949b-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="4949b-108">Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="4949b-108">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="4949b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4949b-109">Permissions</span></span>

<span data-ttu-id="4949b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4949b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4949b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4949b-112">Permission type</span></span>                        | <span data-ttu-id="4949b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4949b-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4949b-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4949b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4949b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4949b-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4949b-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4949b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4949b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4949b-117">Not supported.</span></span>                           |
| <span data-ttu-id="4949b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4949b-118">Application</span></span>                            | <span data-ttu-id="4949b-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4949b-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4949b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4949b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="4949b-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4949b-121">Function parameters</span></span>

<span data-ttu-id="4949b-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4949b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4949b-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4949b-123">Parameter</span></span> | <span data-ttu-id="4949b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="4949b-124">Type</span></span>   | <span data-ttu-id="4949b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4949b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4949b-126">ponto</span><span class="sxs-lookup"><span data-stu-id="4949b-126">period</span></span>    | <span data-ttu-id="4949b-127">string</span><span class="sxs-lookup"><span data-stu-id="4949b-127">string</span></span> | <span data-ttu-id="4949b-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4949b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4949b-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4949b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4949b-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4949b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4949b-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4949b-131">Required.</span></span> |

<span data-ttu-id="4949b-132">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4949b-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4949b-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="4949b-133">The default output type is text/csv.</span></span> <span data-ttu-id="4949b-134">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="4949b-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4949b-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4949b-135">Request headers</span></span>

| <span data-ttu-id="4949b-136">Nome</span><span class="sxs-lookup"><span data-stu-id="4949b-136">Name</span></span>          | <span data-ttu-id="4949b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4949b-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4949b-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="4949b-138">Authorization</span></span> | <span data-ttu-id="4949b-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4949b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4949b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4949b-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4949b-142">CSV</span><span class="sxs-lookup"><span data-stu-id="4949b-142">CSV</span></span>

<span data-ttu-id="4949b-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4949b-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4949b-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4949b-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4949b-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4949b-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4949b-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4949b-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4949b-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4949b-147">Report Refresh Date</span></span>
- <span data-ttu-id="4949b-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4949b-148">Report Date</span></span>
- <span data-ttu-id="4949b-149">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="4949b-149">Team Chat Messages</span></span>
- <span data-ttu-id="4949b-150">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="4949b-150">Private Chat Messages</span></span>
- <span data-ttu-id="4949b-151">Chamadas</span><span class="sxs-lookup"><span data-stu-id="4949b-151">Calls</span></span>
- <span data-ttu-id="4949b-152">Reuniões</span><span class="sxs-lookup"><span data-stu-id="4949b-152">Meetings</span></span>
- <span data-ttu-id="4949b-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4949b-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4949b-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4949b-154">JSON</span></span>

<span data-ttu-id="4949b-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4949b-155">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4949b-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4949b-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4949b-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4949b-157">CSV</span></span>

<span data-ttu-id="4949b-158">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="4949b-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4949b-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4949b-159">Request</span></span>

<span data-ttu-id="4949b-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4949b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4949b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4949b-161">Response</span></span>

<span data-ttu-id="4949b-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4949b-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="4949b-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4949b-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4949b-164">JSON</span><span class="sxs-lookup"><span data-stu-id="4949b-164">JSON</span></span>

<span data-ttu-id="4949b-165">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="4949b-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4949b-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4949b-166">Request</span></span>

<span data-ttu-id="4949b-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4949b-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4949b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4949b-168">Response</span></span>

<span data-ttu-id="4949b-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4949b-169">The following is an example of the response.</span></span>

> <span data-ttu-id="4949b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4949b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
