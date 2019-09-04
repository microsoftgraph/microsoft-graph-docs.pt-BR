---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f30d296caff03e6f572d02a7b9d9149e379ce1ba
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729767"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="c34f4-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="c34f4-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="c34f4-104">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c34f4-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="c34f4-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="c34f4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="c34f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c34f4-106">Permissions</span></span>

<span data-ttu-id="c34f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c34f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c34f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c34f4-109">Permission type</span></span>                        | <span data-ttu-id="c34f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c34f4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c34f4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c34f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c34f4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c34f4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c34f4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c34f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c34f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c34f4-114">Not supported.</span></span>                           |
| <span data-ttu-id="c34f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c34f4-115">Application</span></span>                            | <span data-ttu-id="c34f4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c34f4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c34f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c34f4-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c34f4-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c34f4-118">Function parameters</span></span>

<span data-ttu-id="c34f4-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c34f4-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c34f4-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c34f4-120">Parameter</span></span> | <span data-ttu-id="c34f4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c34f4-121">Type</span></span>   | <span data-ttu-id="c34f4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34f4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c34f4-123">ponto</span><span class="sxs-lookup"><span data-stu-id="c34f4-123">period</span></span>    | <span data-ttu-id="c34f4-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34f4-124">string</span></span> | <span data-ttu-id="c34f4-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c34f4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c34f4-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c34f4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c34f4-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c34f4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c34f4-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c34f4-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c34f4-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c34f4-129">Request headers</span></span>

| <span data-ttu-id="c34f4-130">Nome</span><span class="sxs-lookup"><span data-stu-id="c34f4-130">Name</span></span>          | <span data-ttu-id="c34f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34f4-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c34f4-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="c34f4-132">Authorization</span></span> | <span data-ttu-id="c34f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c34f4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c34f4-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c34f4-135">If-None-Match</span></span> | <span data-ttu-id="c34f4-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="c34f4-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c34f4-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c34f4-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c34f4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c34f4-138">Response</span></span>

<span data-ttu-id="c34f4-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c34f4-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c34f4-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c34f4-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c34f4-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c34f4-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c34f4-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c34f4-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c34f4-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c34f4-143">Report Refresh Date</span></span>
- <span data-ttu-id="c34f4-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="c34f4-144">User Principal Name</span></span>
- <span data-ttu-id="c34f4-145">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c34f4-145">Display Name</span></span>
- <span data-ttu-id="c34f4-146">Excluído</span><span class="sxs-lookup"><span data-stu-id="c34f4-146">Is Deleted</span></span>
- <span data-ttu-id="c34f4-147">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="c34f4-147">Deleted Date</span></span>
- <span data-ttu-id="c34f4-148">Data de criação</span><span class="sxs-lookup"><span data-stu-id="c34f4-148">Created Date</span></span>
- <span data-ttu-id="c34f4-149">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="c34f4-149">Last Activity Date</span></span>
- <span data-ttu-id="c34f4-150">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="c34f4-150">Item Count</span></span>
- <span data-ttu-id="c34f4-151">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="c34f4-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="c34f4-152">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="c34f4-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="c34f4-153">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="c34f4-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="c34f4-154">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="c34f4-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="c34f4-155">Contagem de itens excluídos</span><span class="sxs-lookup"><span data-stu-id="c34f4-155">Deleted Item Count</span></span>
- <span data-ttu-id="c34f4-156">Tamanho de itens excluídos (bytes)</span><span class="sxs-lookup"><span data-stu-id="c34f4-156">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="c34f4-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c34f4-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c34f4-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c34f4-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c34f4-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c34f4-159">Request</span></span>

<span data-ttu-id="c34f4-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c34f4-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c34f4-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="c34f4-161">--Http</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c34f4-162">C#</span><span class="sxs-lookup"><span data-stu-id="c34f4-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c34f4-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c34f4-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c34f4-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c34f4-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c34f4-165">Java</span><span class="sxs-lookup"><span data-stu-id="c34f4-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c34f4-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="c34f4-166">Response</span></span>

<span data-ttu-id="c34f4-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c34f4-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="c34f4-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c34f4-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
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
