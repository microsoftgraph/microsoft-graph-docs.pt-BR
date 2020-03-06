---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 078a06c8cac14a01bea3c3049f115b573f21a4e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510330"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="096a4-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="096a4-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="096a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="096a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="096a4-105">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="096a4-105">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="096a4-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="096a4-106">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="096a4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="096a4-107">Permissions</span></span>

<span data-ttu-id="096a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="096a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="096a4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="096a4-110">Permission type</span></span>                        | <span data-ttu-id="096a4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="096a4-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="096a4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="096a4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="096a4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="096a4-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="096a4-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="096a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="096a4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="096a4-115">Not supported.</span></span>                           |
| <span data-ttu-id="096a4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="096a4-116">Application</span></span>                            | <span data-ttu-id="096a4-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="096a4-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="096a4-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="096a4-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="096a4-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="096a4-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="096a4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="096a4-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="096a4-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="096a4-121">Function parameters</span></span>

<span data-ttu-id="096a4-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="096a4-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="096a4-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="096a4-123">Parameter</span></span> | <span data-ttu-id="096a4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="096a4-124">Type</span></span>   | <span data-ttu-id="096a4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="096a4-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="096a4-126">ponto</span><span class="sxs-lookup"><span data-stu-id="096a4-126">period</span></span>    | <span data-ttu-id="096a4-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="096a4-127">string</span></span> | <span data-ttu-id="096a4-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="096a4-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="096a4-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="096a4-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="096a4-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="096a4-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="096a4-131">data</span><span class="sxs-lookup"><span data-stu-id="096a4-131">date</span></span>      | <span data-ttu-id="096a4-132">Data</span><span class="sxs-lookup"><span data-stu-id="096a4-132">Date</span></span>   | <span data-ttu-id="096a4-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="096a4-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="096a4-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="096a4-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="096a4-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="096a4-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="096a4-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="096a4-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="096a4-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="096a4-137">Request headers</span></span>

| <span data-ttu-id="096a4-138">Nome</span><span class="sxs-lookup"><span data-stu-id="096a4-138">Name</span></span>          | <span data-ttu-id="096a4-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="096a4-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="096a4-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="096a4-140">Authorization</span></span> | <span data-ttu-id="096a4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="096a4-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="096a4-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="096a4-143">If-None-Match</span></span> | <span data-ttu-id="096a4-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="096a4-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="096a4-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="096a4-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="096a4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="096a4-146">Response</span></span>

<span data-ttu-id="096a4-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="096a4-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="096a4-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="096a4-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="096a4-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="096a4-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="096a4-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="096a4-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="096a4-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="096a4-151">Report Refresh Date</span></span>
- <span data-ttu-id="096a4-152">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="096a4-152">Group Display Name</span></span>
- <span data-ttu-id="096a4-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="096a4-153">Is Deleted</span></span>
- <span data-ttu-id="096a4-154">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="096a4-154">Owner Principal Name</span></span>
- <span data-ttu-id="096a4-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="096a4-155">Last Activity Date</span></span>
- <span data-ttu-id="096a4-156">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="096a4-156">Group Type</span></span>
- <span data-ttu-id="096a4-157">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="096a4-157">Member Count</span></span>
- <span data-ttu-id="096a4-158">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="096a4-158">External Member Count</span></span>
- <span data-ttu-id="096a4-159">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="096a4-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="096a4-160">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="096a4-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="096a4-161">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="096a4-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="096a4-162">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="096a4-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="096a4-163">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="096a4-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="096a4-164">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="096a4-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="096a4-165">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="096a4-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="096a4-166">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="096a4-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="096a4-167">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="096a4-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="096a4-168">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="096a4-168">Group Id</span></span>
- <span data-ttu-id="096a4-169">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="096a4-169">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="096a4-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="096a4-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="096a4-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="096a4-171">Request</span></span>

<span data-ttu-id="096a4-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="096a4-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="096a4-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="096a4-173">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="096a4-174">C#</span><span class="sxs-lookup"><span data-stu-id="096a4-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096a4-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096a4-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096a4-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096a4-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096a4-177">Java</span><span class="sxs-lookup"><span data-stu-id="096a4-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="096a4-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="096a4-178">Response</span></span>

<span data-ttu-id="096a4-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="096a4-179">The following is an example of the response.</span></span>

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

<span data-ttu-id="096a4-180">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="096a4-180">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
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
