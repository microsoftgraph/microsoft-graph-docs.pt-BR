---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ea087f2e33238c5268720572c67d2516a9516ece
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510393"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="c44d2-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="c44d2-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="c44d2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c44d2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c44d2-106">Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório.</span><span class="sxs-lookup"><span data-stu-id="c44d2-106">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="c44d2-107">Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.</span><span class="sxs-lookup"><span data-stu-id="c44d2-107">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="c44d2-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="c44d2-108">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="c44d2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c44d2-109">Permissions</span></span>

<span data-ttu-id="c44d2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c44d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c44d2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c44d2-112">Permission type</span></span>                        | <span data-ttu-id="c44d2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c44d2-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c44d2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c44d2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c44d2-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c44d2-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c44d2-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c44d2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c44d2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c44d2-117">Not supported.</span></span>                           |
| <span data-ttu-id="c44d2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c44d2-118">Application</span></span>                            | <span data-ttu-id="c44d2-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c44d2-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="c44d2-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c44d2-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c44d2-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c44d2-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c44d2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c44d2-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c44d2-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c44d2-123">Function parameters</span></span>

<span data-ttu-id="c44d2-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c44d2-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c44d2-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c44d2-125">Parameter</span></span> | <span data-ttu-id="c44d2-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c44d2-126">Type</span></span>   | <span data-ttu-id="c44d2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c44d2-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c44d2-128">ponto</span><span class="sxs-lookup"><span data-stu-id="c44d2-128">period</span></span>    | <span data-ttu-id="c44d2-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c44d2-129">string</span></span> | <span data-ttu-id="c44d2-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c44d2-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c44d2-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c44d2-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c44d2-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c44d2-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c44d2-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c44d2-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c44d2-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c44d2-134">Request headers</span></span>

| <span data-ttu-id="c44d2-135">Nome</span><span class="sxs-lookup"><span data-stu-id="c44d2-135">Name</span></span>          | <span data-ttu-id="c44d2-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c44d2-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c44d2-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="c44d2-137">Authorization</span></span> | <span data-ttu-id="c44d2-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c44d2-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c44d2-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c44d2-140">If-None-Match</span></span> | <span data-ttu-id="c44d2-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="c44d2-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c44d2-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c44d2-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c44d2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c44d2-143">Response</span></span>

<span data-ttu-id="c44d2-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c44d2-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c44d2-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c44d2-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c44d2-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c44d2-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c44d2-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c44d2-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c44d2-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c44d2-148">Report Refresh Date</span></span>
- <span data-ttu-id="c44d2-149">Total</span><span class="sxs-lookup"><span data-stu-id="c44d2-149">Total</span></span>
- <span data-ttu-id="c44d2-150">Ativo</span><span class="sxs-lookup"><span data-stu-id="c44d2-150">Active</span></span>
- <span data-ttu-id="c44d2-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="c44d2-151">Report Date</span></span>
- <span data-ttu-id="c44d2-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c44d2-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c44d2-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c44d2-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c44d2-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c44d2-154">Request</span></span>

<span data-ttu-id="c44d2-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c44d2-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c44d2-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="c44d2-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="c44d2-157">C#</span><span class="sxs-lookup"><span data-stu-id="c44d2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c44d2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c44d2-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c44d2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c44d2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c44d2-160">Java</span><span class="sxs-lookup"><span data-stu-id="c44d2-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c44d2-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c44d2-161">Response</span></span>

<span data-ttu-id="c44d2-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c44d2-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="c44d2-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c44d2-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
