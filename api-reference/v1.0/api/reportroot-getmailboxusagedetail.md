---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2f65cfabdfff4d4892e601d7ddcf253ca6dd6dc5
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982093"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="459d3-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="459d3-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="459d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="459d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="459d3-105">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="459d3-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="459d3-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="459d3-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="459d3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="459d3-107">Permissions</span></span>

<span data-ttu-id="459d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="459d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="459d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="459d3-110">Permission type</span></span>                        | <span data-ttu-id="459d3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="459d3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="459d3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="459d3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="459d3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="459d3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="459d3-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="459d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="459d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="459d3-115">Not supported.</span></span>                           |
| <span data-ttu-id="459d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="459d3-116">Application</span></span>                            | <span data-ttu-id="459d3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="459d3-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="459d3-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="459d3-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="459d3-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="459d3-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="459d3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="459d3-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="459d3-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="459d3-121">Function parameters</span></span>

<span data-ttu-id="459d3-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="459d3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="459d3-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="459d3-123">Parameter</span></span> | <span data-ttu-id="459d3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="459d3-124">Type</span></span>   | <span data-ttu-id="459d3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="459d3-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="459d3-126">ponto</span><span class="sxs-lookup"><span data-stu-id="459d3-126">period</span></span>    | <span data-ttu-id="459d3-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="459d3-127">string</span></span> | <span data-ttu-id="459d3-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="459d3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="459d3-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="459d3-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="459d3-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="459d3-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="459d3-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="459d3-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="459d3-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="459d3-132">Request headers</span></span>

| <span data-ttu-id="459d3-133">Nome</span><span class="sxs-lookup"><span data-stu-id="459d3-133">Name</span></span>          | <span data-ttu-id="459d3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="459d3-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="459d3-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="459d3-135">Authorization</span></span> | <span data-ttu-id="459d3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="459d3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="459d3-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="459d3-138">If-None-Match</span></span> | <span data-ttu-id="459d3-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="459d3-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="459d3-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="459d3-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="459d3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="459d3-141">Response</span></span>

<span data-ttu-id="459d3-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="459d3-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="459d3-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="459d3-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="459d3-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="459d3-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="459d3-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="459d3-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="459d3-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="459d3-146">Report Refresh Date</span></span>
- <span data-ttu-id="459d3-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="459d3-147">User Principal Name</span></span>
- <span data-ttu-id="459d3-148">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="459d3-148">Display Name</span></span>
- <span data-ttu-id="459d3-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="459d3-149">Is Deleted</span></span>
- <span data-ttu-id="459d3-150">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="459d3-150">Deleted Date</span></span>
- <span data-ttu-id="459d3-151">Data de criação</span><span class="sxs-lookup"><span data-stu-id="459d3-151">Created Date</span></span>
- <span data-ttu-id="459d3-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="459d3-152">Last Activity Date</span></span>
- <span data-ttu-id="459d3-153">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="459d3-153">Item Count</span></span>
- <span data-ttu-id="459d3-154">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="459d3-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="459d3-155">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="459d3-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="459d3-156">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="459d3-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="459d3-157">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="459d3-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="459d3-158">Contagem de itens excluídos</span><span class="sxs-lookup"><span data-stu-id="459d3-158">Deleted Item Count</span></span>
- <span data-ttu-id="459d3-159">Tamanho de itens excluídos (bytes)</span><span class="sxs-lookup"><span data-stu-id="459d3-159">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="459d3-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="459d3-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="459d3-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="459d3-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="459d3-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="459d3-162">Request</span></span>

<span data-ttu-id="459d3-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="459d3-163">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="459d3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="459d3-164">Response</span></span>

<span data-ttu-id="459d3-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="459d3-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="459d3-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="459d3-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

