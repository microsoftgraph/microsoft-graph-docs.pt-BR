---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo.
localization_priority: Normal
ms.openlocfilehash: dfd047e4b75191b11f0c8a284c889bd5a6437139
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814774"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="221db-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="221db-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="221db-105">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="221db-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="221db-106">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="221db-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="221db-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="221db-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="221db-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="221db-108">Permissions</span></span>

<span data-ttu-id="221db-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="221db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="221db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="221db-111">Permission type</span></span>                        | <span data-ttu-id="221db-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="221db-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="221db-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="221db-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="221db-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="221db-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="221db-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="221db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="221db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="221db-116">Not supported.</span></span>                           |
| <span data-ttu-id="221db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="221db-117">Application</span></span>                            | <span data-ttu-id="221db-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="221db-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="221db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="221db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="221db-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="221db-120">Function parameters</span></span>

<span data-ttu-id="221db-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="221db-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="221db-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="221db-122">Parameter</span></span> | <span data-ttu-id="221db-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="221db-123">Type</span></span>   | <span data-ttu-id="221db-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="221db-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="221db-125">ponto</span><span class="sxs-lookup"><span data-stu-id="221db-125">period</span></span>    | <span data-ttu-id="221db-126">string</span><span class="sxs-lookup"><span data-stu-id="221db-126">string</span></span> | <span data-ttu-id="221db-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="221db-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="221db-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="221db-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="221db-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="221db-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="221db-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="221db-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="221db-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="221db-131">Request headers</span></span>

| <span data-ttu-id="221db-132">Nome</span><span class="sxs-lookup"><span data-stu-id="221db-132">Name</span></span>          | <span data-ttu-id="221db-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="221db-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="221db-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="221db-134">Authorization</span></span> | <span data-ttu-id="221db-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="221db-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="221db-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="221db-137">If-None-Match</span></span> | <span data-ttu-id="221db-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="221db-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="221db-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="221db-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="221db-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="221db-140">Response</span></span>

<span data-ttu-id="221db-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="221db-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="221db-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="221db-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="221db-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="221db-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="221db-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="221db-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="221db-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="221db-145">Report Refresh Date</span></span>
- <span data-ttu-id="221db-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="221db-146">Report Date</span></span>
- <span data-ttu-id="221db-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="221db-147">Report Period</span></span>
- <span data-ttu-id="221db-148">Áudio</span><span class="sxs-lookup"><span data-stu-id="221db-148">Audio</span></span>
- <span data-ttu-id="221db-149">Vídeo</span><span class="sxs-lookup"><span data-stu-id="221db-149">Video</span></span>

## <a name="example"></a><span data-ttu-id="221db-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="221db-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="221db-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="221db-151">Request</span></span>

<span data-ttu-id="221db-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="221db-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="221db-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="221db-153">Response</span></span>

<span data-ttu-id="221db-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="221db-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="221db-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="221db-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```
