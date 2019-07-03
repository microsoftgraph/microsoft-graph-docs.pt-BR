---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a1803b9c92054126161329dc997e5270bcca6cf6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445209"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="7c56b-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="7c56b-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="7c56b-104">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="7c56b-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="7c56b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="7c56b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c56b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c56b-106">Permissions</span></span>

<span data-ttu-id="7c56b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c56b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c56b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c56b-109">Permission type</span></span>                        | <span data-ttu-id="7c56b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c56b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c56b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c56b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c56b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c56b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c56b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c56b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c56b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c56b-114">Not supported.</span></span>                           |
| <span data-ttu-id="7c56b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c56b-115">Application</span></span>                            | <span data-ttu-id="7c56b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c56b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c56b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c56b-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7c56b-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c56b-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7c56b-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7c56b-119">Function parameters</span></span>

<span data-ttu-id="7c56b-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7c56b-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7c56b-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7c56b-121">Parameter</span></span> | <span data-ttu-id="7c56b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c56b-122">Type</span></span>   | <span data-ttu-id="7c56b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c56b-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c56b-124">ponto</span><span class="sxs-lookup"><span data-stu-id="7c56b-124">period</span></span>    | <span data-ttu-id="7c56b-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c56b-125">string</span></span> | <span data-ttu-id="7c56b-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7c56b-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c56b-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7c56b-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c56b-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7c56b-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7c56b-129">data</span><span class="sxs-lookup"><span data-stu-id="7c56b-129">date</span></span>      | <span data-ttu-id="7c56b-130">Data</span><span class="sxs-lookup"><span data-stu-id="7c56b-130">Date</span></span>   | <span data-ttu-id="7c56b-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="7c56b-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7c56b-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7c56b-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7c56b-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7c56b-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7c56b-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="7c56b-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c56b-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c56b-135">Request headers</span></span>

| <span data-ttu-id="7c56b-136">Nome</span><span class="sxs-lookup"><span data-stu-id="7c56b-136">Name</span></span>          | <span data-ttu-id="7c56b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c56b-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7c56b-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c56b-138">Authorization</span></span> | <span data-ttu-id="7c56b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c56b-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7c56b-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7c56b-141">If-None-Match</span></span> | <span data-ttu-id="7c56b-142">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="7c56b-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7c56b-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7c56b-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7c56b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c56b-144">Response</span></span>

<span data-ttu-id="7c56b-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7c56b-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c56b-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7c56b-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c56b-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7c56b-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c56b-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7c56b-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c56b-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7c56b-149">Report Refresh Date</span></span>
- <span data-ttu-id="7c56b-150">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="7c56b-150">Group Display Name</span></span>
- <span data-ttu-id="7c56b-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="7c56b-151">Is Deleted</span></span>
- <span data-ttu-id="7c56b-152">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="7c56b-152">Owner Principal Name</span></span>
- <span data-ttu-id="7c56b-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="7c56b-153">Last Activity Date</span></span>
- <span data-ttu-id="7c56b-154">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="7c56b-154">Group Type</span></span>
- <span data-ttu-id="7c56b-155">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="7c56b-155">Member Count</span></span>
- <span data-ttu-id="7c56b-156">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="7c56b-156">External Member Count</span></span>
- <span data-ttu-id="7c56b-157">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="7c56b-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="7c56b-158">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="7c56b-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="7c56b-159">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="7c56b-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="7c56b-160">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="7c56b-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="7c56b-161">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="7c56b-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="7c56b-162">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="7c56b-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="7c56b-163">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="7c56b-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="7c56b-164">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="7c56b-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="7c56b-165">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="7c56b-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="7c56b-166">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7c56b-166">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7c56b-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c56b-167">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c56b-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c56b-168">Request</span></span>

<span data-ttu-id="7c56b-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c56b-169">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c56b-170">C#</span><span class="sxs-lookup"><span data-stu-id="7c56b-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c56b-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c56b-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c56b-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7c56b-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c56b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c56b-173">Response</span></span>

<span data-ttu-id="7c56b-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c56b-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="7c56b-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7c56b-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
