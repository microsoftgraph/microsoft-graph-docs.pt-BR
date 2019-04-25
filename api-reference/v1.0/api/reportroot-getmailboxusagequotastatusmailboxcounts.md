---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: da947184ece4be0015829f19243753bd39695745
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574219"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="15f79-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="15f79-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="15f79-104">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="15f79-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="15f79-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="15f79-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="15f79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15f79-106">Permissions</span></span>

<span data-ttu-id="15f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15f79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15f79-109">Permission type</span></span>                        | <span data-ttu-id="15f79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15f79-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="15f79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15f79-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="15f79-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15f79-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="15f79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15f79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15f79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15f79-114">Not supported.</span></span>                           |
| <span data-ttu-id="15f79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15f79-115">Application</span></span>                            | <span data-ttu-id="15f79-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15f79-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="15f79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15f79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="15f79-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="15f79-118">Function parameters</span></span>

<span data-ttu-id="15f79-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="15f79-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="15f79-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="15f79-120">Parameter</span></span> | <span data-ttu-id="15f79-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="15f79-121">Type</span></span>   | <span data-ttu-id="15f79-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f79-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="15f79-123">ponto</span><span class="sxs-lookup"><span data-stu-id="15f79-123">period</span></span>    | <span data-ttu-id="15f79-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15f79-124">string</span></span> | <span data-ttu-id="15f79-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="15f79-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="15f79-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="15f79-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="15f79-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="15f79-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="15f79-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15f79-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="15f79-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15f79-129">Request headers</span></span>

| <span data-ttu-id="15f79-130">Nome</span><span class="sxs-lookup"><span data-stu-id="15f79-130">Name</span></span>          | <span data-ttu-id="15f79-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f79-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="15f79-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="15f79-132">Authorization</span></span> | <span data-ttu-id="15f79-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15f79-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="15f79-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="15f79-135">If-None-Match</span></span> | <span data-ttu-id="15f79-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="15f79-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="15f79-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="15f79-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="15f79-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f79-138">Response</span></span>

<span data-ttu-id="15f79-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="15f79-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="15f79-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="15f79-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="15f79-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="15f79-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="15f79-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="15f79-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="15f79-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="15f79-143">Report Refresh Date</span></span>
- <span data-ttu-id="15f79-144">Abaixo do limite</span><span class="sxs-lookup"><span data-stu-id="15f79-144">Under Limit</span></span>
- <span data-ttu-id="15f79-145">Aviso emitido</span><span class="sxs-lookup"><span data-stu-id="15f79-145">Warning Issued</span></span>
- <span data-ttu-id="15f79-146">Envio proibido</span><span class="sxs-lookup"><span data-stu-id="15f79-146">Send Prohibited</span></span>
- <span data-ttu-id="15f79-147">Envio/recebimento proibido</span><span class="sxs-lookup"><span data-stu-id="15f79-147">Send/Receive Prohibited</span></span>
- <span data-ttu-id="15f79-148">Indeterminado</span><span class="sxs-lookup"><span data-stu-id="15f79-148">Indeterminate</span></span>
- <span data-ttu-id="15f79-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="15f79-149">Report Date</span></span>
- <span data-ttu-id="15f79-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="15f79-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="15f79-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15f79-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="15f79-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f79-152">Request</span></span>

<span data-ttu-id="15f79-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15f79-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="15f79-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f79-154">Response</span></span>

<span data-ttu-id="15f79-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15f79-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="15f79-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="15f79-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```
