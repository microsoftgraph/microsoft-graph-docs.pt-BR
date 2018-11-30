---
title: 'reportRoot: getYammerActivityUserCounts'
description: Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.
ms.openlocfilehash: bdac79d93f2506f4781948cef0eeb27d9f0a99c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007043"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="08a95-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="08a95-103">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="08a95-104">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="08a95-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="08a95-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="08a95-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="08a95-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="08a95-106">Permissions</span></span>

<span data-ttu-id="08a95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08a95-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08a95-109">Permission type</span></span>                        | <span data-ttu-id="08a95-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08a95-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08a95-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08a95-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08a95-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08a95-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08a95-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08a95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08a95-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08a95-114">Not supported.</span></span>                           |
| <span data-ttu-id="08a95-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08a95-115">Application</span></span>                            | <span data-ttu-id="08a95-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08a95-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="08a95-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08a95-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="08a95-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="08a95-118">Function parameters</span></span>

<span data-ttu-id="08a95-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="08a95-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="08a95-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08a95-120">Parameter</span></span> | <span data-ttu-id="08a95-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="08a95-121">Type</span></span>   | <span data-ttu-id="08a95-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a95-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08a95-123">ponto</span><span class="sxs-lookup"><span data-stu-id="08a95-123">period</span></span>    | <span data-ttu-id="08a95-124">string</span><span class="sxs-lookup"><span data-stu-id="08a95-124">string</span></span> | <span data-ttu-id="08a95-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="08a95-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08a95-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="08a95-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08a95-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="08a95-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="08a95-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a95-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="08a95-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08a95-129">Request headers</span></span>

| <span data-ttu-id="08a95-130">Nome</span><span class="sxs-lookup"><span data-stu-id="08a95-130">Name</span></span>          | <span data-ttu-id="08a95-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a95-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="08a95-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="08a95-132">Authorization</span></span> | <span data-ttu-id="08a95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a95-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="08a95-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="08a95-135">If-None-Match</span></span> | <span data-ttu-id="08a95-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="08a95-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="08a95-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="08a95-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="08a95-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a95-138">Response</span></span>

<span data-ttu-id="08a95-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="08a95-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08a95-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="08a95-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08a95-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="08a95-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08a95-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="08a95-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08a95-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="08a95-143">Report Refresh Date</span></span>
- <span data-ttu-id="08a95-144">Curtidos</span><span class="sxs-lookup"><span data-stu-id="08a95-144">Liked</span></span>
- <span data-ttu-id="08a95-145">Postados</span><span class="sxs-lookup"><span data-stu-id="08a95-145">Posted</span></span>
- <span data-ttu-id="08a95-146">Ler</span><span class="sxs-lookup"><span data-stu-id="08a95-146">Read</span></span>
- <span data-ttu-id="08a95-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="08a95-147">Report Date</span></span>
- <span data-ttu-id="08a95-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="08a95-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="08a95-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08a95-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08a95-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08a95-150">Request</span></span>

<span data-ttu-id="08a95-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a95-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="08a95-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a95-152">Response</span></span>

<span data-ttu-id="08a95-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08a95-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="08a95-154">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="08a95-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
