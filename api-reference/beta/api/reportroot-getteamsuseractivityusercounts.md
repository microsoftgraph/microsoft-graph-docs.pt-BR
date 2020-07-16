---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8c895b60774b4c8d0496e9702c8f0202f7b43acb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896141"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="1458c-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1458c-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="1458c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1458c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1458c-106">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="1458c-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="1458c-107">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="1458c-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="1458c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1458c-108">Permissions</span></span>

<span data-ttu-id="1458c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1458c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1458c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1458c-111">Permission type</span></span>                        | <span data-ttu-id="1458c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1458c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1458c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1458c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1458c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1458c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1458c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1458c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1458c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1458c-116">Not supported.</span></span>                           |
| <span data-ttu-id="1458c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1458c-117">Application</span></span>                            | <span data-ttu-id="1458c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1458c-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="1458c-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="1458c-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1458c-120">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="1458c-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1458c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1458c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="1458c-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1458c-122">Function parameters</span></span>

<span data-ttu-id="1458c-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1458c-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1458c-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1458c-124">Parameter</span></span> | <span data-ttu-id="1458c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="1458c-125">Type</span></span>   | <span data-ttu-id="1458c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1458c-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1458c-127">ponto</span><span class="sxs-lookup"><span data-stu-id="1458c-127">period</span></span>    | <span data-ttu-id="1458c-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1458c-128">string</span></span> | <span data-ttu-id="1458c-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1458c-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1458c-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1458c-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1458c-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1458c-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1458c-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1458c-132">Required.</span></span> |

<span data-ttu-id="1458c-133">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1458c-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1458c-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1458c-134">The default output type is text/csv.</span></span> <span data-ttu-id="1458c-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1458c-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1458c-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1458c-136">Request headers</span></span>

| <span data-ttu-id="1458c-137">Nome</span><span class="sxs-lookup"><span data-stu-id="1458c-137">Name</span></span>          | <span data-ttu-id="1458c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1458c-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1458c-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="1458c-139">Authorization</span></span> | <span data-ttu-id="1458c-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1458c-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1458c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1458c-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1458c-143">CSV</span><span class="sxs-lookup"><span data-stu-id="1458c-143">CSV</span></span>

<span data-ttu-id="1458c-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1458c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1458c-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1458c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1458c-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1458c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1458c-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1458c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1458c-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1458c-148">Report Refresh Date</span></span>
- <span data-ttu-id="1458c-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1458c-149">Report Date</span></span>
- <span data-ttu-id="1458c-150">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="1458c-150">Team Chat Messages</span></span>
- <span data-ttu-id="1458c-151">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="1458c-151">Private Chat Messages</span></span>
- <span data-ttu-id="1458c-152">Chamadas</span><span class="sxs-lookup"><span data-stu-id="1458c-152">Calls</span></span>
- <span data-ttu-id="1458c-153">Reuniões</span><span class="sxs-lookup"><span data-stu-id="1458c-153">Meetings</span></span>
- <span data-ttu-id="1458c-154">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="1458c-154">Other Actions</span></span>
- <span data-ttu-id="1458c-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1458c-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1458c-156">JSON</span><span class="sxs-lookup"><span data-stu-id="1458c-156">JSON</span></span>

<span data-ttu-id="1458c-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1458c-157">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1458c-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1458c-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1458c-159">CSV</span><span class="sxs-lookup"><span data-stu-id="1458c-159">CSV</span></span>

<span data-ttu-id="1458c-160">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1458c-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1458c-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1458c-161">Request</span></span>

<span data-ttu-id="1458c-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1458c-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="1458c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1458c-163">Response</span></span>

<span data-ttu-id="1458c-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1458c-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1458c-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1458c-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1458c-166">JSON</span><span class="sxs-lookup"><span data-stu-id="1458c-166">JSON</span></span>

<span data-ttu-id="1458c-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1458c-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1458c-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1458c-168">Request</span></span>

<span data-ttu-id="1458c-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1458c-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="1458c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="1458c-170">Response</span></span>

<span data-ttu-id="1458c-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1458c-171">The following is an example of the response.</span></span>

> <span data-ttu-id="1458c-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1458c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
