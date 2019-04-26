---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 15ed192eab2641dd91354726812ae4d4f528c71a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336464"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="1a1b0-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="1a1b0-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a1b0-105">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="1a1b0-106">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="1a1b0-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="1a1b0-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a1b0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a1b0-108">Permissions</span></span>

<span data-ttu-id="1a1b0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a1b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a1b0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a1b0-111">Permission type</span></span>                        | <span data-ttu-id="1a1b0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a1b0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1a1b0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a1b0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a1b0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a1b0-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1a1b0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a1b0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a1b0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-116">Not supported.</span></span>                           |
| <span data-ttu-id="1a1b0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a1b0-117">Application</span></span>                            | <span data-ttu-id="1a1b0-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a1b0-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1a1b0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a1b0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1a1b0-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1a1b0-120">Function parameters</span></span>

<span data-ttu-id="1a1b0-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1a1b0-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1a1b0-122">Parameter</span></span> | <span data-ttu-id="1a1b0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1b0-123">Type</span></span>   | <span data-ttu-id="1a1b0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1b0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1a1b0-125">ponto</span><span class="sxs-lookup"><span data-stu-id="1a1b0-125">period</span></span>    | <span data-ttu-id="1a1b0-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1b0-126">string</span></span> | <span data-ttu-id="1a1b0-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1a1b0-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1a1b0-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1a1b0-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-130">Required.</span></span> |

<span data-ttu-id="1a1b0-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1a1b0-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-132">The default output type is text/csv.</span></span> <span data-ttu-id="1a1b0-133">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a1b0-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1b0-134">Request headers</span></span>

| <span data-ttu-id="1a1b0-135">Nome</span><span class="sxs-lookup"><span data-stu-id="1a1b0-135">Name</span></span>          | <span data-ttu-id="1a1b0-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1b0-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1a1b0-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a1b0-137">Authorization</span></span> | <span data-ttu-id="1a1b0-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1a1b0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1b0-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1a1b0-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1a1b0-141">CSV</span></span>

<span data-ttu-id="1a1b0-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1a1b0-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1a1b0-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1a1b0-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1a1b0-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1a1b0-146">Report Refresh Date</span></span>
- <span data-ttu-id="1a1b0-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1a1b0-147">Report Date</span></span>
- <span data-ttu-id="1a1b0-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1a1b0-148">Report Period</span></span>
- <span data-ttu-id="1a1b0-149">Áudio</span><span class="sxs-lookup"><span data-stu-id="1a1b0-149">Audio</span></span>
- <span data-ttu-id="1a1b0-150">Vídeo</span><span class="sxs-lookup"><span data-stu-id="1a1b0-150">Video</span></span>

### <a name="json"></a><span data-ttu-id="1a1b0-151">JSON</span><span class="sxs-lookup"><span data-stu-id="1a1b0-151">JSON</span></span>

<span data-ttu-id="1a1b0-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-152">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1b0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a1b0-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1a1b0-154">CSV</span><span class="sxs-lookup"><span data-stu-id="1a1b0-154">CSV</span></span>

<span data-ttu-id="1a1b0-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1a1b0-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1b0-156">Request</span></span>

<span data-ttu-id="1a1b0-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1a1b0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1b0-158">Response</span></span>

<span data-ttu-id="1a1b0-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1a1b0-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="1a1b0-161">JSON</span><span class="sxs-lookup"><span data-stu-id="1a1b0-161">JSON</span></span>

<span data-ttu-id="1a1b0-162">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1a1b0-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a1b0-163">Request</span></span>

<span data-ttu-id="1a1b0-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1a1b0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a1b0-165">Response</span></span>

<span data-ttu-id="1a1b0-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-166">The following is an example of the response.</span></span>

> <span data-ttu-id="1a1b0-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a1b0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
