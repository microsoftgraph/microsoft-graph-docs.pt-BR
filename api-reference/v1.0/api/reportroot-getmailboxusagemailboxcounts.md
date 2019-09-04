---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0d7736edaccdf976c8adda3816dcc5c68bb2e74c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728241"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="bdcc2-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="bdcc2-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="bdcc2-105">Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="bdcc2-106">Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="bdcc2-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="bdcc2-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdcc2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdcc2-108">Permissions</span></span>

<span data-ttu-id="bdcc2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdcc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdcc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdcc2-111">Permission type</span></span>                        | <span data-ttu-id="bdcc2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdcc2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bdcc2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdcc2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdcc2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdcc2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bdcc2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdcc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdcc2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-116">Not supported.</span></span>                           |
| <span data-ttu-id="bdcc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdcc2-117">Application</span></span>                            | <span data-ttu-id="bdcc2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdcc2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bdcc2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdcc2-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bdcc2-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bdcc2-120">Function parameters</span></span>

<span data-ttu-id="bdcc2-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bdcc2-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bdcc2-122">Parameter</span></span> | <span data-ttu-id="bdcc2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdcc2-123">Type</span></span>   | <span data-ttu-id="bdcc2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdcc2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bdcc2-125">ponto</span><span class="sxs-lookup"><span data-stu-id="bdcc2-125">period</span></span>    | <span data-ttu-id="bdcc2-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdcc2-126">string</span></span> | <span data-ttu-id="bdcc2-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bdcc2-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bdcc2-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bdcc2-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bdcc2-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcc2-131">Request headers</span></span>

| <span data-ttu-id="bdcc2-132">Nome</span><span class="sxs-lookup"><span data-stu-id="bdcc2-132">Name</span></span>          | <span data-ttu-id="bdcc2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdcc2-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bdcc2-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdcc2-134">Authorization</span></span> | <span data-ttu-id="bdcc2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bdcc2-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bdcc2-137">If-None-Match</span></span> | <span data-ttu-id="bdcc2-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bdcc2-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bdcc2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdcc2-140">Response</span></span>

<span data-ttu-id="bdcc2-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bdcc2-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bdcc2-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bdcc2-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bdcc2-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bdcc2-145">Report Refresh Date</span></span>
- <span data-ttu-id="bdcc2-146">Total</span><span class="sxs-lookup"><span data-stu-id="bdcc2-146">Total</span></span>
- <span data-ttu-id="bdcc2-147">Ativo</span><span class="sxs-lookup"><span data-stu-id="bdcc2-147">Active</span></span>
- <span data-ttu-id="bdcc2-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="bdcc2-148">Report Date</span></span>
- <span data-ttu-id="bdcc2-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bdcc2-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bdcc2-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdcc2-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bdcc2-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcc2-151">Request</span></span>

<span data-ttu-id="bdcc2-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bdcc2-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdcc2-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bdcc2-154">C#</span><span class="sxs-lookup"><span data-stu-id="bdcc2-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdcc2-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdcc2-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdcc2-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bdcc2-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bdcc2-157">Java</span><span class="sxs-lookup"><span data-stu-id="bdcc2-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bdcc2-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdcc2-158">Response</span></span>

<span data-ttu-id="bdcc2-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="bdcc2-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bdcc2-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
