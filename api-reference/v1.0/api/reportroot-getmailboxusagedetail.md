---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: a4f412d8acdb32648ceb47e4aed6f2b7ff83268d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953480"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="0c284-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="0c284-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="0c284-104">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0c284-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="0c284-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="0c284-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c284-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c284-106">Permissions</span></span>

<span data-ttu-id="0c284-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c284-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c284-109">Permission type</span></span>                        | <span data-ttu-id="0c284-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c284-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0c284-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c284-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c284-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c284-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0c284-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c284-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c284-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c284-114">Not supported.</span></span>                           |
| <span data-ttu-id="0c284-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c284-115">Application</span></span>                            | <span data-ttu-id="0c284-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c284-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0c284-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c284-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0c284-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0c284-118">Function parameters</span></span>

<span data-ttu-id="0c284-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0c284-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0c284-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0c284-120">Parameter</span></span> | <span data-ttu-id="0c284-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c284-121">Type</span></span>   | <span data-ttu-id="0c284-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c284-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0c284-123">ponto</span><span class="sxs-lookup"><span data-stu-id="0c284-123">period</span></span>    | <span data-ttu-id="0c284-124">string</span><span class="sxs-lookup"><span data-stu-id="0c284-124">string</span></span> | <span data-ttu-id="0c284-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0c284-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0c284-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0c284-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0c284-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0c284-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0c284-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c284-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0c284-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c284-129">Request headers</span></span>

| <span data-ttu-id="0c284-130">Nome</span><span class="sxs-lookup"><span data-stu-id="0c284-130">Name</span></span>          | <span data-ttu-id="0c284-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c284-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0c284-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c284-132">Authorization</span></span> | <span data-ttu-id="0c284-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c284-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0c284-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0c284-135">If-None-Match</span></span> | <span data-ttu-id="0c284-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="0c284-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0c284-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0c284-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0c284-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c284-138">Response</span></span>

<span data-ttu-id="0c284-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0c284-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0c284-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0c284-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0c284-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0c284-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0c284-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0c284-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0c284-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0c284-143">Report Refresh Date</span></span>
- <span data-ttu-id="0c284-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="0c284-144">User Principal Name</span></span>
- <span data-ttu-id="0c284-145">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="0c284-145">Display Name</span></span>
- <span data-ttu-id="0c284-146">Excluído</span><span class="sxs-lookup"><span data-stu-id="0c284-146">Is Deleted</span></span>
- <span data-ttu-id="0c284-147">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="0c284-147">Deleted Date</span></span>
- <span data-ttu-id="0c284-148">Data de criação</span><span class="sxs-lookup"><span data-stu-id="0c284-148">Created Date</span></span>
- <span data-ttu-id="0c284-149">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="0c284-149">Last Activity Date</span></span>
- <span data-ttu-id="0c284-150">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="0c284-150">Item Count</span></span>
- <span data-ttu-id="0c284-151">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="0c284-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="0c284-152">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="0c284-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="0c284-153">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="0c284-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="0c284-154">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="0c284-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="0c284-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0c284-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0c284-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c284-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0c284-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c284-157">Request</span></span>

<span data-ttu-id="0c284-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c284-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0c284-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c284-159">Response</span></span>

<span data-ttu-id="0c284-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c284-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="0c284-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0c284-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```
