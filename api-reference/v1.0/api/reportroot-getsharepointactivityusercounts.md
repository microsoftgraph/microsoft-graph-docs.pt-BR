---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 09b0b823858d34212aa0580c3c85f645734bf901
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525436"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="ad241-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ad241-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="ad241-105">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="ad241-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="ad241-106">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="ad241-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="ad241-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="ad241-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad241-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad241-108">Permissions</span></span>

<span data-ttu-id="ad241-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad241-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad241-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad241-111">Permission type</span></span>                        | <span data-ttu-id="ad241-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad241-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad241-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad241-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad241-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad241-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad241-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad241-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad241-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad241-116">Not supported.</span></span>                           |
| <span data-ttu-id="ad241-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad241-117">Application</span></span>                            | <span data-ttu-id="ad241-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad241-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ad241-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad241-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ad241-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ad241-120">Function parameters</span></span>

<span data-ttu-id="ad241-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ad241-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ad241-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ad241-122">Parameter</span></span> | <span data-ttu-id="ad241-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad241-123">Type</span></span>   | <span data-ttu-id="ad241-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad241-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad241-125">ponto</span><span class="sxs-lookup"><span data-stu-id="ad241-125">period</span></span>    | <span data-ttu-id="ad241-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad241-126">string</span></span> | <span data-ttu-id="ad241-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ad241-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad241-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ad241-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad241-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ad241-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ad241-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad241-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ad241-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad241-131">Request headers</span></span>

| <span data-ttu-id="ad241-132">Nome</span><span class="sxs-lookup"><span data-stu-id="ad241-132">Name</span></span>          | <span data-ttu-id="ad241-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad241-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ad241-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad241-134">Authorization</span></span> | <span data-ttu-id="ad241-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad241-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ad241-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ad241-137">If-None-Match</span></span> | <span data-ttu-id="ad241-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ad241-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ad241-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad241-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ad241-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad241-140">Response</span></span>

<span data-ttu-id="ad241-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ad241-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad241-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ad241-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad241-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ad241-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad241-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ad241-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad241-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ad241-145">Report Refresh Date</span></span>
- <span data-ttu-id="ad241-146">Página visitada</span><span class="sxs-lookup"><span data-stu-id="ad241-146">Visited Page</span></span>
- <span data-ttu-id="ad241-147">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="ad241-147">Viewed Or Edited</span></span>
- <span data-ttu-id="ad241-148">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="ad241-148">Synced</span></span>
- <span data-ttu-id="ad241-149">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="ad241-149">Shared Internally</span></span>
- <span data-ttu-id="ad241-150">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="ad241-150">Shared Externally</span></span>
- <span data-ttu-id="ad241-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ad241-151">Report Date</span></span>
- <span data-ttu-id="ad241-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ad241-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ad241-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad241-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ad241-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad241-154">Request</span></span>

<span data-ttu-id="ad241-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad241-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ad241-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad241-156">Response</span></span>

<span data-ttu-id="ad241-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad241-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="ad241-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ad241-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
