---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
ms.openlocfilehash: 927d9511a5190b2aa5540c6046c8162e5fa5f9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005603"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="5c1e0-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="5c1e0-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="5c1e0-104">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="5c1e0-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="5c1e0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c1e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c1e0-106">Permissions</span></span>

<span data-ttu-id="5c1e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c1e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c1e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c1e0-109">Permission type</span></span>                        | <span data-ttu-id="5c1e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c1e0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5c1e0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c1e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c1e0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c1e0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5c1e0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c1e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c1e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-114">Not supported.</span></span>                           |
| <span data-ttu-id="5c1e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c1e0-115">Application</span></span>                            | <span data-ttu-id="5c1e0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c1e0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5c1e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c1e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5c1e0-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5c1e0-118">Function parameters</span></span>

<span data-ttu-id="5c1e0-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5c1e0-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c1e0-120">Parameter</span></span> | <span data-ttu-id="5c1e0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c1e0-121">Type</span></span>   | <span data-ttu-id="5c1e0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c1e0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5c1e0-123">ponto</span><span class="sxs-lookup"><span data-stu-id="5c1e0-123">period</span></span>    | <span data-ttu-id="5c1e0-124">string</span><span class="sxs-lookup"><span data-stu-id="5c1e0-124">string</span></span> | <span data-ttu-id="5c1e0-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5c1e0-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5c1e0-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5c1e0-128">data</span><span class="sxs-lookup"><span data-stu-id="5c1e0-128">date</span></span>      | <span data-ttu-id="5c1e0-129">Data</span><span class="sxs-lookup"><span data-stu-id="5c1e0-129">Date</span></span>   | <span data-ttu-id="5c1e0-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5c1e0-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5c1e0-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5c1e0-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c1e0-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e0-134">Request headers</span></span>

| <span data-ttu-id="5c1e0-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5c1e0-135">Name</span></span>          | <span data-ttu-id="5c1e0-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c1e0-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5c1e0-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c1e0-137">Authorization</span></span> | <span data-ttu-id="5c1e0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5c1e0-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5c1e0-140">If-None-Match</span></span> | <span data-ttu-id="5c1e0-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5c1e0-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5c1e0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1e0-143">Response</span></span>

<span data-ttu-id="5c1e0-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5c1e0-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5c1e0-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5c1e0-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5c1e0-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5c1e0-148">Report Refresh Date</span></span>
- <span data-ttu-id="5c1e0-149">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="5c1e0-149">Group Display Name</span></span>
- <span data-ttu-id="5c1e0-150">Excluído</span><span class="sxs-lookup"><span data-stu-id="5c1e0-150">Is Deleted</span></span>
- <span data-ttu-id="5c1e0-151">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="5c1e0-151">Owner Principal Name</span></span>
- <span data-ttu-id="5c1e0-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="5c1e0-152">Last Activity Date</span></span>
- <span data-ttu-id="5c1e0-153">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="5c1e0-153">Group Type</span></span>
- <span data-ttu-id="5c1e0-154">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="5c1e0-154">Office 365 Connected</span></span>
- <span data-ttu-id="5c1e0-155">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="5c1e0-155">Member Count</span></span>
- <span data-ttu-id="5c1e0-156">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="5c1e0-156">Posted Count</span></span>
- <span data-ttu-id="5c1e0-157">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="5c1e0-157">Read Count</span></span>
- <span data-ttu-id="5c1e0-158">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="5c1e0-158">Liked Count</span></span>
- <span data-ttu-id="5c1e0-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5c1e0-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5c1e0-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c1e0-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5c1e0-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e0-161">Request</span></span>

<span data-ttu-id="5c1e0-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5c1e0-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1e0-163">Response</span></span>

<span data-ttu-id="5c1e0-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-164">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="5c1e0-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e0-165">Request</span></span>
<span data-ttu-id="5c1e0-166">Se for chamado com um `date`, o relatório destinado a atividade na data especificada.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-166">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="5c1e0-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1e0-167">Response</span></span>

<span data-ttu-id="5c1e0-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5c1e0-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5c1e0-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
