---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.
ms.openlocfilehash: cacc2b99b841a9775aa6b2b6a67ed03cf0cd82a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003783"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="385bc-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="385bc-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="385bc-104">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="385bc-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="385bc-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="385bc-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="385bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="385bc-106">Permissions</span></span>

<span data-ttu-id="385bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="385bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="385bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="385bc-109">Permission type</span></span>                        | <span data-ttu-id="385bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="385bc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="385bc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="385bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="385bc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="385bc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="385bc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="385bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="385bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="385bc-114">Not supported.</span></span>                           |
| <span data-ttu-id="385bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="385bc-115">Application</span></span>                            | <span data-ttu-id="385bc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="385bc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="385bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="385bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="385bc-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="385bc-118">Function parameters</span></span>

<span data-ttu-id="385bc-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="385bc-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="385bc-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="385bc-120">Parameter</span></span> | <span data-ttu-id="385bc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="385bc-121">Type</span></span>   | <span data-ttu-id="385bc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="385bc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="385bc-123">ponto</span><span class="sxs-lookup"><span data-stu-id="385bc-123">period</span></span>    | <span data-ttu-id="385bc-124">string</span><span class="sxs-lookup"><span data-stu-id="385bc-124">string</span></span> | <span data-ttu-id="385bc-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="385bc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="385bc-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="385bc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="385bc-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="385bc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="385bc-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="385bc-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="385bc-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="385bc-129">Request headers</span></span>

| <span data-ttu-id="385bc-130">Nome</span><span class="sxs-lookup"><span data-stu-id="385bc-130">Name</span></span>          | <span data-ttu-id="385bc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="385bc-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="385bc-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="385bc-132">Authorization</span></span> | <span data-ttu-id="385bc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="385bc-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="385bc-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="385bc-135">If-None-Match</span></span> | <span data-ttu-id="385bc-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="385bc-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="385bc-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="385bc-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="385bc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="385bc-138">Response</span></span>

<span data-ttu-id="385bc-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="385bc-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="385bc-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="385bc-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="385bc-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="385bc-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="385bc-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="385bc-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="385bc-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="385bc-143">Report Refresh Date</span></span>
- <span data-ttu-id="385bc-144">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="385bc-144">Viewed Or Edited</span></span>
- <span data-ttu-id="385bc-145">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="385bc-145">Synced</span></span>
- <span data-ttu-id="385bc-146">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="385bc-146">Shared Internally</span></span>
- <span data-ttu-id="385bc-147">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="385bc-147">Shared Externally</span></span>
- <span data-ttu-id="385bc-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="385bc-148">Report Date</span></span>
- <span data-ttu-id="385bc-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="385bc-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="385bc-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="385bc-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="385bc-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="385bc-151">Request</span></span>

<span data-ttu-id="385bc-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="385bc-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="385bc-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="385bc-153">Response</span></span>

<span data-ttu-id="385bc-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="385bc-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="385bc-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="385bc-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
