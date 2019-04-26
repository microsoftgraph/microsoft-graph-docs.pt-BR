---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 556b9d7ebe8fcd4d113fe6c7f25793c59b093e2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331844"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="ed8d9-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ed8d9-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed8d9-105">Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="ed8d9-106">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="ed8d9-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="ed8d9-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed8d9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed8d9-108">Permissions</span></span>

<span data-ttu-id="ed8d9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed8d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed8d9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed8d9-111">Permission type</span></span>                        | <span data-ttu-id="ed8d9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed8d9-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ed8d9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed8d9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed8d9-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8d9-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ed8d9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed8d9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed8d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-116">Not supported.</span></span>                           |
| <span data-ttu-id="ed8d9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed8d9-117">Application</span></span>                            | <span data-ttu-id="ed8d9-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8d9-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ed8d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed8d9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ed8d9-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ed8d9-120">Function parameters</span></span>

<span data-ttu-id="ed8d9-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ed8d9-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ed8d9-122">Parameter</span></span> | <span data-ttu-id="ed8d9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed8d9-123">Type</span></span>   | <span data-ttu-id="ed8d9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed8d9-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ed8d9-125">ponto</span><span class="sxs-lookup"><span data-stu-id="ed8d9-125">period</span></span>    | <span data-ttu-id="ed8d9-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed8d9-126">string</span></span> | <span data-ttu-id="ed8d9-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ed8d9-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ed8d9-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ed8d9-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-130">Required.</span></span> |

<span data-ttu-id="ed8d9-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ed8d9-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-132">The default output type is text/csv.</span></span> <span data-ttu-id="ed8d9-133">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed8d9-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed8d9-134">Request headers</span></span>

| <span data-ttu-id="ed8d9-135">Nome</span><span class="sxs-lookup"><span data-stu-id="ed8d9-135">Name</span></span>          | <span data-ttu-id="ed8d9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed8d9-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ed8d9-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed8d9-137">Authorization</span></span> | <span data-ttu-id="ed8d9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ed8d9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed8d9-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ed8d9-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ed8d9-141">CSV</span></span>

<span data-ttu-id="ed8d9-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ed8d9-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ed8d9-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ed8d9-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ed8d9-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ed8d9-146">Report Refresh Date</span></span>
- <span data-ttu-id="ed8d9-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ed8d9-147">Report Date</span></span>
- <span data-ttu-id="ed8d9-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ed8d9-148">Report Period</span></span>
- <span data-ttu-id="ed8d9-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="ed8d9-149">IM</span></span>
- <span data-ttu-id="ed8d9-150">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="ed8d9-150">Audio/Video</span></span>
- <span data-ttu-id="ed8d9-151">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="ed8d9-151">App Sharing</span></span>
- <span data-ttu-id="ed8d9-152">Web</span><span class="sxs-lookup"><span data-stu-id="ed8d9-152">Web</span></span>
- <span data-ttu-id="ed8d9-153">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="ed8d9-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="ed8d9-154">JSON</span><span class="sxs-lookup"><span data-stu-id="ed8d9-154">JSON</span></span>

<span data-ttu-id="ed8d9-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed8d9-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed8d9-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ed8d9-157">CSV</span><span class="sxs-lookup"><span data-stu-id="ed8d9-157">CSV</span></span>

<span data-ttu-id="ed8d9-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ed8d9-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed8d9-159">Request</span></span>

<span data-ttu-id="ed8d9-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ed8d9-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed8d9-161">Response</span></span>

<span data-ttu-id="ed8d9-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ed8d9-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="ed8d9-164">JSON</span><span class="sxs-lookup"><span data-stu-id="ed8d9-164">JSON</span></span>

<span data-ttu-id="ed8d9-165">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ed8d9-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed8d9-166">Request</span></span>

<span data-ttu-id="ed8d9-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ed8d9-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed8d9-168">Response</span></span>

<span data-ttu-id="ed8d9-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-169">The following is an example of the response.</span></span>

> <span data-ttu-id="ed8d9-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed8d9-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
