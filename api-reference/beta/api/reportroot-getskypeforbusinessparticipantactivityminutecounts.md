---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8f7f1953241753ac1170216db1a590ea7e4be8d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945885"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="77acf-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="77acf-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

> <span data-ttu-id="77acf-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77acf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77acf-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77acf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77acf-107">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="77acf-107">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="77acf-108">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="77acf-108">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="77acf-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="77acf-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="77acf-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="77acf-110">Permissions</span></span>

<span data-ttu-id="77acf-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77acf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77acf-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77acf-113">Permission type</span></span>                        | <span data-ttu-id="77acf-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77acf-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="77acf-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77acf-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="77acf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="77acf-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="77acf-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77acf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77acf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77acf-118">Not supported.</span></span>                           |
| <span data-ttu-id="77acf-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77acf-119">Application</span></span>                            | <span data-ttu-id="77acf-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="77acf-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="77acf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77acf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="77acf-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="77acf-122">Function parameters</span></span>

<span data-ttu-id="77acf-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="77acf-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="77acf-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77acf-124">Parameter</span></span> | <span data-ttu-id="77acf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="77acf-125">Type</span></span>   | <span data-ttu-id="77acf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="77acf-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="77acf-127">ponto</span><span class="sxs-lookup"><span data-stu-id="77acf-127">period</span></span>    | <span data-ttu-id="77acf-128">string</span><span class="sxs-lookup"><span data-stu-id="77acf-128">string</span></span> | <span data-ttu-id="77acf-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="77acf-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="77acf-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="77acf-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="77acf-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="77acf-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="77acf-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77acf-132">Required.</span></span> |

<span data-ttu-id="77acf-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="77acf-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="77acf-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="77acf-134">The default output type is text/csv.</span></span> <span data-ttu-id="77acf-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="77acf-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77acf-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77acf-136">Request headers</span></span>

| <span data-ttu-id="77acf-137">Nome</span><span class="sxs-lookup"><span data-stu-id="77acf-137">Name</span></span>          | <span data-ttu-id="77acf-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="77acf-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="77acf-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="77acf-139">Authorization</span></span> | <span data-ttu-id="77acf-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77acf-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="77acf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="77acf-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="77acf-143">CSV</span><span class="sxs-lookup"><span data-stu-id="77acf-143">CSV</span></span>

<span data-ttu-id="77acf-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="77acf-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="77acf-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="77acf-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="77acf-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="77acf-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="77acf-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="77acf-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="77acf-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="77acf-148">Report Refresh Date</span></span>
- <span data-ttu-id="77acf-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="77acf-149">Report Date</span></span>
- <span data-ttu-id="77acf-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="77acf-150">Report Period</span></span>
- <span data-ttu-id="77acf-151">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="77acf-151">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="77acf-152">JSON</span><span class="sxs-lookup"><span data-stu-id="77acf-152">JSON</span></span>

<span data-ttu-id="77acf-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77acf-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77acf-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77acf-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="77acf-155">CSV</span><span class="sxs-lookup"><span data-stu-id="77acf-155">CSV</span></span>

<span data-ttu-id="77acf-156">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="77acf-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="77acf-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77acf-157">Request</span></span>

<span data-ttu-id="77acf-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77acf-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="77acf-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="77acf-159">Response</span></span>

<span data-ttu-id="77acf-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77acf-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="77acf-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="77acf-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```

### <a name="json"></a><span data-ttu-id="77acf-162">JSON</span><span class="sxs-lookup"><span data-stu-id="77acf-162">JSON</span></span>

<span data-ttu-id="77acf-163">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="77acf-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="77acf-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77acf-164">Request</span></span>

<span data-ttu-id="77acf-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77acf-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="77acf-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="77acf-166">Response</span></span>

<span data-ttu-id="77acf-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77acf-167">The following is an example of the response.</span></span>

> <span data-ttu-id="77acf-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77acf-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts)", 
  "value": [
    {
      "audiovideo": 6267, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
