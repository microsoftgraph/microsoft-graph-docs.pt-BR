---
title: 'reportRoot: getSharePointActivityPages'
description: Obtenha o número de páginas exclusivas visitadas pelos usuários.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a361e17ad4d82b9f0c9c4dab80186e9970e59210
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525569"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="3b345-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="3b345-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="3b345-104">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="3b345-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="3b345-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="3b345-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b345-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b345-106">Permissions</span></span>

<span data-ttu-id="3b345-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b345-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b345-109">Permission type</span></span>                        | <span data-ttu-id="3b345-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b345-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3b345-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b345-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b345-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b345-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3b345-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b345-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b345-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b345-114">Not supported.</span></span>                           |
| <span data-ttu-id="3b345-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b345-115">Application</span></span>                            | <span data-ttu-id="3b345-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b345-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3b345-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b345-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3b345-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3b345-118">Function parameters</span></span>

<span data-ttu-id="3b345-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3b345-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3b345-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3b345-120">Parameter</span></span> | <span data-ttu-id="3b345-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b345-121">Type</span></span>   | <span data-ttu-id="3b345-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b345-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3b345-123">ponto</span><span class="sxs-lookup"><span data-stu-id="3b345-123">period</span></span>    | <span data-ttu-id="3b345-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b345-124">string</span></span> | <span data-ttu-id="3b345-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3b345-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3b345-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3b345-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3b345-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3b345-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3b345-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b345-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3b345-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b345-129">Request headers</span></span>

| <span data-ttu-id="3b345-130">Nome</span><span class="sxs-lookup"><span data-stu-id="3b345-130">Name</span></span>          | <span data-ttu-id="3b345-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b345-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3b345-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b345-132">Authorization</span></span> | <span data-ttu-id="3b345-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b345-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3b345-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3b345-135">If-None-Match</span></span> | <span data-ttu-id="3b345-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3b345-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3b345-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3b345-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3b345-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b345-138">Response</span></span>

<span data-ttu-id="3b345-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3b345-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3b345-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3b345-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3b345-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3b345-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3b345-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3b345-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3b345-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3b345-143">Report Refresh Date</span></span>
- <span data-ttu-id="3b345-144">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="3b345-144">Visited Page Count</span></span>
- <span data-ttu-id="3b345-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3b345-145">Report Date</span></span>
- <span data-ttu-id="3b345-146">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3b345-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3b345-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b345-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3b345-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b345-148">Request</span></span>

<span data-ttu-id="3b345-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b345-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivitypages"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityPages(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3b345-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b345-150">Response</span></span>

<span data-ttu-id="3b345-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b345-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="3b345-152">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3b345-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```
