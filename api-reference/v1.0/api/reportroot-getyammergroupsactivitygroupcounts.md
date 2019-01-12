---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d0daae8bab7ddce1fa6412d064429b40b290a044
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954264"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="702fb-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="702fb-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

<span data-ttu-id="702fb-104">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="702fb-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="702fb-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="702fb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="702fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="702fb-106">Permissions</span></span>

<span data-ttu-id="702fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="702fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="702fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="702fb-109">Permission type</span></span>                        | <span data-ttu-id="702fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="702fb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="702fb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="702fb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="702fb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="702fb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="702fb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="702fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="702fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="702fb-114">Not supported.</span></span>                           |
| <span data-ttu-id="702fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="702fb-115">Application</span></span>                            | <span data-ttu-id="702fb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="702fb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="702fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="702fb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="702fb-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="702fb-118">Function parameters</span></span>

<span data-ttu-id="702fb-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="702fb-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="702fb-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="702fb-120">Parameter</span></span> | <span data-ttu-id="702fb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="702fb-121">Type</span></span>   | <span data-ttu-id="702fb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="702fb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="702fb-123">ponto</span><span class="sxs-lookup"><span data-stu-id="702fb-123">period</span></span>    | <span data-ttu-id="702fb-124">string</span><span class="sxs-lookup"><span data-stu-id="702fb-124">string</span></span> | <span data-ttu-id="702fb-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="702fb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="702fb-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="702fb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="702fb-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="702fb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="702fb-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="702fb-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="702fb-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="702fb-129">Request headers</span></span>

| <span data-ttu-id="702fb-130">Nome</span><span class="sxs-lookup"><span data-stu-id="702fb-130">Name</span></span>          | <span data-ttu-id="702fb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="702fb-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="702fb-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="702fb-132">Authorization</span></span> | <span data-ttu-id="702fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="702fb-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="702fb-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="702fb-135">If-None-Match</span></span> | <span data-ttu-id="702fb-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="702fb-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="702fb-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="702fb-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="702fb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="702fb-138">Response</span></span>

<span data-ttu-id="702fb-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="702fb-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="702fb-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="702fb-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="702fb-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="702fb-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="702fb-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="702fb-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="702fb-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="702fb-143">Report Refresh Date</span></span>
- <span data-ttu-id="702fb-144">Total</span><span class="sxs-lookup"><span data-stu-id="702fb-144">Total</span></span>
- <span data-ttu-id="702fb-145">Ativo</span><span class="sxs-lookup"><span data-stu-id="702fb-145">Active</span></span>
- <span data-ttu-id="702fb-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="702fb-146">Report Date</span></span>
- <span data-ttu-id="702fb-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="702fb-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="702fb-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="702fb-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="702fb-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="702fb-149">Request</span></span>

<span data-ttu-id="702fb-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="702fb-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitygroupcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityGroupCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="702fb-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="702fb-151">Response</span></span>

<span data-ttu-id="702fb-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="702fb-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="702fb-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="702fb-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
