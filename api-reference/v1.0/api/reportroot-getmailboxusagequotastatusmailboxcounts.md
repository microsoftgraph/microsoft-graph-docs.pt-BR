---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f567f86a58940e67065ba8f0c9d5c97642fb4fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327257"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="0f465-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="0f465-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="0f465-104">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="0f465-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="0f465-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="0f465-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f465-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f465-106">Permissions</span></span>

<span data-ttu-id="0f465-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f465-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f465-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f465-109">Permission type</span></span>                        | <span data-ttu-id="0f465-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f465-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0f465-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f465-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f465-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f465-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0f465-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f465-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f465-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f465-114">Not supported.</span></span>                           |
| <span data-ttu-id="0f465-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f465-115">Application</span></span>                            | <span data-ttu-id="0f465-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f465-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0f465-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f465-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0f465-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0f465-118">Function parameters</span></span>

<span data-ttu-id="0f465-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0f465-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0f465-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0f465-120">Parameter</span></span> | <span data-ttu-id="0f465-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f465-121">Type</span></span>   | <span data-ttu-id="0f465-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f465-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0f465-123">ponto</span><span class="sxs-lookup"><span data-stu-id="0f465-123">period</span></span>    | <span data-ttu-id="0f465-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f465-124">string</span></span> | <span data-ttu-id="0f465-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0f465-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0f465-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0f465-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0f465-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0f465-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0f465-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f465-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0f465-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f465-129">Request headers</span></span>

| <span data-ttu-id="0f465-130">Nome</span><span class="sxs-lookup"><span data-stu-id="0f465-130">Name</span></span>          | <span data-ttu-id="0f465-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f465-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0f465-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f465-132">Authorization</span></span> | <span data-ttu-id="0f465-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f465-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0f465-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0f465-135">If-None-Match</span></span> | <span data-ttu-id="0f465-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="0f465-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0f465-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0f465-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0f465-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f465-138">Response</span></span>

<span data-ttu-id="0f465-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0f465-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0f465-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0f465-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0f465-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0f465-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0f465-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0f465-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0f465-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0f465-143">Report Refresh Date</span></span>
- <span data-ttu-id="0f465-144">Abaixo do limite</span><span class="sxs-lookup"><span data-stu-id="0f465-144">Under Limit</span></span>
- <span data-ttu-id="0f465-145">Aviso emitido</span><span class="sxs-lookup"><span data-stu-id="0f465-145">Warning Issued</span></span>
- <span data-ttu-id="0f465-146">Envio proibido</span><span class="sxs-lookup"><span data-stu-id="0f465-146">Send Prohibited</span></span>
- <span data-ttu-id="0f465-147">Envio/recebimento proibido</span><span class="sxs-lookup"><span data-stu-id="0f465-147">Send/Receive Prohibited</span></span>
- <span data-ttu-id="0f465-148">Indeterminado</span><span class="sxs-lookup"><span data-stu-id="0f465-148">Indeterminate</span></span>
- <span data-ttu-id="0f465-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="0f465-149">Report Date</span></span>
- <span data-ttu-id="0f465-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0f465-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0f465-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f465-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0f465-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f465-152">Request</span></span>

<span data-ttu-id="0f465-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f465-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0f465-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f465-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f465-155">C#</span><span class="sxs-lookup"><span data-stu-id="0f465-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f465-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f465-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f465-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f465-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0f465-158">Java</span><span class="sxs-lookup"><span data-stu-id="0f465-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f465-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f465-159">Response</span></span>

<span data-ttu-id="0f465-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f465-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="0f465-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0f465-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
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
  ]
}-->
