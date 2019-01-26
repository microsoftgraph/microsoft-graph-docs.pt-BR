---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0b642c581522197661b73c6b5ea7765b79b02366
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571699"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="5cae9-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5cae9-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="5cae9-104">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="5cae9-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="5cae9-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="5cae9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cae9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5cae9-106">Permissions</span></span>

<span data-ttu-id="5cae9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5cae9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cae9-109">Permission type</span></span>                        | <span data-ttu-id="5cae9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5cae9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5cae9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cae9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cae9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cae9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5cae9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cae9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cae9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cae9-114">Not supported.</span></span>                           |
| <span data-ttu-id="5cae9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cae9-115">Application</span></span>                            | <span data-ttu-id="5cae9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cae9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5cae9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cae9-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5cae9-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5cae9-118">Function parameters</span></span>

<span data-ttu-id="5cae9-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5cae9-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5cae9-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5cae9-120">Parameter</span></span> | <span data-ttu-id="5cae9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cae9-121">Type</span></span>   | <span data-ttu-id="5cae9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cae9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5cae9-123">ponto</span><span class="sxs-lookup"><span data-stu-id="5cae9-123">period</span></span>    | <span data-ttu-id="5cae9-124">string</span><span class="sxs-lookup"><span data-stu-id="5cae9-124">string</span></span> | <span data-ttu-id="5cae9-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5cae9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5cae9-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5cae9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5cae9-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5cae9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5cae9-128">data</span><span class="sxs-lookup"><span data-stu-id="5cae9-128">date</span></span>      | <span data-ttu-id="5cae9-129">Data</span><span class="sxs-lookup"><span data-stu-id="5cae9-129">Date</span></span>   | <span data-ttu-id="5cae9-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="5cae9-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5cae9-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="5cae9-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5cae9-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5cae9-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5cae9-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="5cae9-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cae9-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cae9-134">Request headers</span></span>

| <span data-ttu-id="5cae9-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5cae9-135">Name</span></span>          | <span data-ttu-id="5cae9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cae9-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5cae9-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cae9-137">Authorization</span></span> | <span data-ttu-id="5cae9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cae9-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5cae9-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5cae9-140">If-None-Match</span></span> | <span data-ttu-id="5cae9-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5cae9-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5cae9-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5cae9-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5cae9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cae9-143">Response</span></span>

<span data-ttu-id="5cae9-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5cae9-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5cae9-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5cae9-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5cae9-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5cae9-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5cae9-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5cae9-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5cae9-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5cae9-148">Report Refresh Date</span></span>
- <span data-ttu-id="5cae9-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="5cae9-149">User Principal Name</span></span>
- <span data-ttu-id="5cae9-150">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="5cae9-150">Display Name</span></span>
- <span data-ttu-id="5cae9-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="5cae9-151">Is Deleted</span></span>
- <span data-ttu-id="5cae9-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="5cae9-152">Deleted Date</span></span>
- <span data-ttu-id="5cae9-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="5cae9-153">Last Activity Date</span></span>
- <span data-ttu-id="5cae9-154">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="5cae9-154">Mail For Mac</span></span>
- <span data-ttu-id="5cae9-155">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="5cae9-155">Outlook For Mac</span></span>
- <span data-ttu-id="5cae9-156">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="5cae9-156">Outlook For Windows</span></span>
- <span data-ttu-id="5cae9-157">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="5cae9-157">Outlook For Mobile</span></span>
- <span data-ttu-id="5cae9-158">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="5cae9-158">Other For Mobile</span></span>
- <span data-ttu-id="5cae9-159">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="5cae9-159">Outlook For Web</span></span>
- <span data-ttu-id="5cae9-160">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="5cae9-160">POP3 App</span></span>
- <span data-ttu-id="5cae9-161">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="5cae9-161">IMAP4 App</span></span>
- <span data-ttu-id="5cae9-162">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="5cae9-162">SMTP App</span></span>
- <span data-ttu-id="5cae9-163">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5cae9-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5cae9-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cae9-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5cae9-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cae9-165">Request</span></span>

<span data-ttu-id="5cae9-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cae9-166">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5cae9-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cae9-167">Response</span></span>

<span data-ttu-id="5cae9-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5cae9-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="5cae9-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5cae9-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
