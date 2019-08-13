---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cb2165cd8e010fe47682853605d6e8724550d6d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326636"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="3d60c-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="3d60c-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="3d60c-104">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="3d60c-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="3d60c-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="3d60c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d60c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d60c-106">Permissions</span></span>

<span data-ttu-id="3d60c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d60c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d60c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d60c-109">Permission type</span></span>                        | <span data-ttu-id="3d60c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d60c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3d60c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d60c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d60c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d60c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3d60c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d60c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d60c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d60c-114">Not supported.</span></span>                           |
| <span data-ttu-id="3d60c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d60c-115">Application</span></span>                            | <span data-ttu-id="3d60c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d60c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3d60c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d60c-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3d60c-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3d60c-118">Function parameters</span></span>

<span data-ttu-id="3d60c-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3d60c-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3d60c-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3d60c-120">Parameter</span></span> | <span data-ttu-id="3d60c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d60c-121">Type</span></span>   | <span data-ttu-id="3d60c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d60c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3d60c-123">ponto</span><span class="sxs-lookup"><span data-stu-id="3d60c-123">period</span></span>    | <span data-ttu-id="3d60c-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d60c-124">string</span></span> | <span data-ttu-id="3d60c-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3d60c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3d60c-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3d60c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3d60c-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3d60c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3d60c-128">data</span><span class="sxs-lookup"><span data-stu-id="3d60c-128">date</span></span>      | <span data-ttu-id="3d60c-129">Data</span><span class="sxs-lookup"><span data-stu-id="3d60c-129">Date</span></span>   | <span data-ttu-id="3d60c-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="3d60c-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3d60c-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="3d60c-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3d60c-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="3d60c-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3d60c-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="3d60c-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d60c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d60c-134">Request headers</span></span>

| <span data-ttu-id="3d60c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="3d60c-135">Name</span></span>          | <span data-ttu-id="3d60c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d60c-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3d60c-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d60c-137">Authorization</span></span> | <span data-ttu-id="3d60c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d60c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3d60c-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3d60c-140">If-None-Match</span></span> | <span data-ttu-id="3d60c-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3d60c-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3d60c-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d60c-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3d60c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d60c-143">Response</span></span>

<span data-ttu-id="3d60c-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3d60c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3d60c-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3d60c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3d60c-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3d60c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3d60c-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3d60c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3d60c-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3d60c-148">Report Refresh Date</span></span>
- <span data-ttu-id="3d60c-149">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="3d60c-149">Group Display Name</span></span>
- <span data-ttu-id="3d60c-150">Excluído</span><span class="sxs-lookup"><span data-stu-id="3d60c-150">Is Deleted</span></span>
- <span data-ttu-id="3d60c-151">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="3d60c-151">Owner Principal Name</span></span>
- <span data-ttu-id="3d60c-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="3d60c-152">Last Activity Date</span></span>
- <span data-ttu-id="3d60c-153">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="3d60c-153">Group Type</span></span>
- <span data-ttu-id="3d60c-154">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="3d60c-154">Member Count</span></span>
- <span data-ttu-id="3d60c-155">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="3d60c-155">External Member Count</span></span>
- <span data-ttu-id="3d60c-156">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="3d60c-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="3d60c-157">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="3d60c-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="3d60c-158">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="3d60c-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="3d60c-159">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="3d60c-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="3d60c-160">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="3d60c-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="3d60c-161">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="3d60c-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="3d60c-162">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="3d60c-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="3d60c-163">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="3d60c-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="3d60c-164">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="3d60c-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="3d60c-165">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3d60c-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3d60c-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d60c-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3d60c-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d60c-167">Request</span></span>

<span data-ttu-id="3d60c-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d60c-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3d60c-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d60c-169">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d60c-170">C#</span><span class="sxs-lookup"><span data-stu-id="3d60c-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d60c-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d60c-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d60c-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3d60c-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3d60c-173">Java</span><span class="sxs-lookup"><span data-stu-id="3d60c-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3d60c-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d60c-174">Response</span></span>

<span data-ttu-id="3d60c-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d60c-175">The following is an example of the response.</span></span>

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

<span data-ttu-id="3d60c-176">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3d60c-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
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
