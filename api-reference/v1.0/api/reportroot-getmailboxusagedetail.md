---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c7b29395486962d8387ffb438465c6f63adf9042
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268793"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="dbb33-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="dbb33-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="dbb33-104">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="dbb33-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="dbb33-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="dbb33-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="dbb33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbb33-106">Permissions</span></span>

<span data-ttu-id="dbb33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbb33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbb33-109">Permission type</span></span>                        | <span data-ttu-id="dbb33-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbb33-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dbb33-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbb33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbb33-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbb33-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dbb33-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbb33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbb33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbb33-114">Not supported.</span></span>                           |
| <span data-ttu-id="dbb33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbb33-115">Application</span></span>                            | <span data-ttu-id="dbb33-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbb33-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dbb33-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbb33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dbb33-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="dbb33-118">Function parameters</span></span>

<span data-ttu-id="dbb33-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="dbb33-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dbb33-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dbb33-120">Parameter</span></span> | <span data-ttu-id="dbb33-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb33-121">Type</span></span>   | <span data-ttu-id="dbb33-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb33-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dbb33-123">ponto</span><span class="sxs-lookup"><span data-stu-id="dbb33-123">period</span></span>    | <span data-ttu-id="dbb33-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb33-124">string</span></span> | <span data-ttu-id="dbb33-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dbb33-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dbb33-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="dbb33-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dbb33-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dbb33-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dbb33-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb33-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dbb33-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb33-129">Request headers</span></span>

| <span data-ttu-id="dbb33-130">Nome</span><span class="sxs-lookup"><span data-stu-id="dbb33-130">Name</span></span>          | <span data-ttu-id="dbb33-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb33-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dbb33-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbb33-132">Authorization</span></span> | <span data-ttu-id="dbb33-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb33-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dbb33-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dbb33-135">If-None-Match</span></span> | <span data-ttu-id="dbb33-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="dbb33-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dbb33-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dbb33-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dbb33-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb33-138">Response</span></span>

<span data-ttu-id="dbb33-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dbb33-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dbb33-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dbb33-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dbb33-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dbb33-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dbb33-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="dbb33-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dbb33-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dbb33-143">Report Refresh Date</span></span>
- <span data-ttu-id="dbb33-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="dbb33-144">User Principal Name</span></span>
- <span data-ttu-id="dbb33-145">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="dbb33-145">Display Name</span></span>
- <span data-ttu-id="dbb33-146">Excluído</span><span class="sxs-lookup"><span data-stu-id="dbb33-146">Is Deleted</span></span>
- <span data-ttu-id="dbb33-147">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="dbb33-147">Deleted Date</span></span>
- <span data-ttu-id="dbb33-148">Data de criação</span><span class="sxs-lookup"><span data-stu-id="dbb33-148">Created Date</span></span>
- <span data-ttu-id="dbb33-149">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="dbb33-149">Last Activity Date</span></span>
- <span data-ttu-id="dbb33-150">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="dbb33-150">Item Count</span></span>
- <span data-ttu-id="dbb33-151">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="dbb33-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="dbb33-152">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="dbb33-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="dbb33-153">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="dbb33-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="dbb33-154">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="dbb33-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="dbb33-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="dbb33-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dbb33-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbb33-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dbb33-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb33-157">Request</span></span>

<span data-ttu-id="dbb33-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbb33-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="dbb33-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb33-159">Response</span></span>

<span data-ttu-id="dbb33-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dbb33-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dbb33-161">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="dbb33-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dbb33-162">C#</span><span class="sxs-lookup"><span data-stu-id="dbb33-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbb33-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbb33-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dbb33-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbb33-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusageuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="dbb33-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dbb33-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
