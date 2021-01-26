---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obter detalhes sobre a atividade de grupos do Microsoft 365 por grupo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 059a2b3bfb35545df66ea68015f5b68354e332e6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981736"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="9b710-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="9b710-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="9b710-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b710-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b710-105">Obter detalhes sobre a atividade de grupos do Microsoft 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="9b710-105">Get details about Microsoft 365 groups activity by group.</span></span>

> <span data-ttu-id="9b710-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - grupos do Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="9b710-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b710-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b710-107">Permissions</span></span>

<span data-ttu-id="9b710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b710-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b710-110">Permission type</span></span>                        | <span data-ttu-id="9b710-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b710-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9b710-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b710-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b710-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b710-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9b710-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b710-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b710-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b710-115">Not supported.</span></span>                           |
| <span data-ttu-id="9b710-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b710-116">Application</span></span>                            | <span data-ttu-id="9b710-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b710-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="9b710-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9b710-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9b710-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="9b710-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9b710-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b710-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9b710-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9b710-121">Function parameters</span></span>

<span data-ttu-id="9b710-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9b710-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9b710-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9b710-123">Parameter</span></span> | <span data-ttu-id="9b710-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b710-124">Type</span></span>   | <span data-ttu-id="9b710-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b710-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9b710-126">ponto</span><span class="sxs-lookup"><span data-stu-id="9b710-126">period</span></span>    | <span data-ttu-id="9b710-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b710-127">string</span></span> | <span data-ttu-id="9b710-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9b710-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9b710-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9b710-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9b710-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9b710-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9b710-131">data</span><span class="sxs-lookup"><span data-stu-id="9b710-131">date</span></span>      | <span data-ttu-id="9b710-132">Data</span><span class="sxs-lookup"><span data-stu-id="9b710-132">Date</span></span>   | <span data-ttu-id="9b710-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="9b710-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9b710-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9b710-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9b710-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9b710-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9b710-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="9b710-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b710-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b710-137">Request headers</span></span>

| <span data-ttu-id="9b710-138">Nome</span><span class="sxs-lookup"><span data-stu-id="9b710-138">Name</span></span>          | <span data-ttu-id="9b710-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b710-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9b710-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b710-140">Authorization</span></span> | <span data-ttu-id="9b710-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b710-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9b710-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9b710-143">If-None-Match</span></span> | <span data-ttu-id="9b710-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="9b710-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9b710-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9b710-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9b710-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b710-146">Response</span></span>

<span data-ttu-id="9b710-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9b710-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9b710-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9b710-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9b710-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9b710-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9b710-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9b710-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9b710-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9b710-151">Report Refresh Date</span></span>
- <span data-ttu-id="9b710-152">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="9b710-152">Group Display Name</span></span>
- <span data-ttu-id="9b710-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="9b710-153">Is Deleted</span></span>
- <span data-ttu-id="9b710-154">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="9b710-154">Owner Principal Name</span></span>
- <span data-ttu-id="9b710-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="9b710-155">Last Activity Date</span></span>
- <span data-ttu-id="9b710-156">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="9b710-156">Group Type</span></span>
- <span data-ttu-id="9b710-157">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="9b710-157">Member Count</span></span>
- <span data-ttu-id="9b710-158">Contagem de membros externos</span><span class="sxs-lookup"><span data-stu-id="9b710-158">External Member Count</span></span>
- <span data-ttu-id="9b710-159">Contagem de emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b710-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="9b710-160">Contagem de arquivos ativos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="9b710-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="9b710-161">Contagem de mensagens postadas no Yammer</span><span class="sxs-lookup"><span data-stu-id="9b710-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="9b710-162">Contagem de mensagens lidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="9b710-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="9b710-163">Contagem de mensagens curtidas no Yammer</span><span class="sxs-lookup"><span data-stu-id="9b710-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="9b710-164">Quantidade de itens totais da caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b710-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="9b710-165">Armazenamento utilizado da caixa de correio do Exchange (bytes)</span><span class="sxs-lookup"><span data-stu-id="9b710-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="9b710-166">Contagem total de arquivos do SharePoint</span><span class="sxs-lookup"><span data-stu-id="9b710-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="9b710-167">Armazenamento utilizado do site do SharePoint (bytes)</span><span class="sxs-lookup"><span data-stu-id="9b710-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="9b710-168">ID do Grupo</span><span class="sxs-lookup"><span data-stu-id="9b710-168">Group Id</span></span>
- <span data-ttu-id="9b710-169">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9b710-169">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9b710-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b710-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9b710-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b710-171">Request</span></span>

<span data-ttu-id="9b710-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b710-172">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="9b710-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b710-173">Response</span></span>

<span data-ttu-id="9b710-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b710-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="9b710-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9b710-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

