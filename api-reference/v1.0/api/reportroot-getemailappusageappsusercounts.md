---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Obtenha a contagem de usuários únicos por aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 071dde5c18a6b30cda502c121cde65a5dd69e0a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582308"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="8793d-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="8793d-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="8793d-104">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="8793d-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="8793d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="8793d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8793d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8793d-106">Permissions</span></span>

<span data-ttu-id="8793d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8793d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8793d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8793d-109">Permission type</span></span>                        | <span data-ttu-id="8793d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8793d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8793d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8793d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8793d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8793d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8793d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8793d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8793d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8793d-114">Not supported.</span></span>                           |
| <span data-ttu-id="8793d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8793d-115">Application</span></span>                            | <span data-ttu-id="8793d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8793d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8793d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8793d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8793d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8793d-118">Function parameters</span></span>

<span data-ttu-id="8793d-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8793d-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8793d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8793d-120">Parameter</span></span> | <span data-ttu-id="8793d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8793d-121">Type</span></span>   | <span data-ttu-id="8793d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8793d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8793d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="8793d-123">period</span></span>    | <span data-ttu-id="8793d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8793d-124">string</span></span> | <span data-ttu-id="8793d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8793d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8793d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8793d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8793d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8793d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8793d-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8793d-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8793d-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8793d-129">Request headers</span></span>

| <span data-ttu-id="8793d-130">Nome</span><span class="sxs-lookup"><span data-stu-id="8793d-130">Name</span></span>          | <span data-ttu-id="8793d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8793d-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8793d-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="8793d-132">Authorization</span></span> | <span data-ttu-id="8793d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8793d-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8793d-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8793d-135">If-None-Match</span></span> | <span data-ttu-id="8793d-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="8793d-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8793d-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8793d-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8793d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8793d-138">Response</span></span>

<span data-ttu-id="8793d-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8793d-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8793d-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8793d-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8793d-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8793d-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8793d-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8793d-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8793d-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8793d-143">Report Refresh Date</span></span>
- <span data-ttu-id="8793d-144">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="8793d-144">Mail For Mac</span></span>
- <span data-ttu-id="8793d-145">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="8793d-145">Outlook For Mac</span></span>
- <span data-ttu-id="8793d-146">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="8793d-146">Outlook For Windows</span></span>
- <span data-ttu-id="8793d-147">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="8793d-147">Outlook For Mobile</span></span>
- <span data-ttu-id="8793d-148">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="8793d-148">Other For Mobile</span></span>
- <span data-ttu-id="8793d-149">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="8793d-149">Outlook For Web</span></span>
- <span data-ttu-id="8793d-150">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="8793d-150">POP3 App</span></span>
- <span data-ttu-id="8793d-151">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="8793d-151">IMAP4 App</span></span>
- <span data-ttu-id="8793d-152">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="8793d-152">SMTP App</span></span>
- <span data-ttu-id="8793d-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8793d-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8793d-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8793d-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8793d-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8793d-155">Request</span></span>

<span data-ttu-id="8793d-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8793d-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8793d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8793d-157">Response</span></span>

<span data-ttu-id="8793d-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8793d-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="8793d-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8793d-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
