---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Obtenha dados sobre as atividades do SharePoint por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: cee105e804c66b7bdbe1101b27f07b89616d0e08
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983185"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="d1ea5-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d1ea5-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="d1ea5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1ea5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1ea5-105">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-105">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="d1ea5-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="d1ea5-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1ea5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1ea5-107">Permissions</span></span>

<span data-ttu-id="d1ea5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1ea5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1ea5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1ea5-110">Permission type</span></span>                        | <span data-ttu-id="d1ea5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1ea5-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d1ea5-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1ea5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1ea5-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1ea5-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d1ea5-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1ea5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1ea5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-115">Not supported.</span></span>                           |
| <span data-ttu-id="d1ea5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1ea5-116">Application</span></span>                            | <span data-ttu-id="d1ea5-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1ea5-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d1ea5-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d1ea5-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d1ea5-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d1ea5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1ea5-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d1ea5-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d1ea5-121">Function parameters</span></span>

<span data-ttu-id="d1ea5-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d1ea5-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d1ea5-123">Parameter</span></span> | <span data-ttu-id="d1ea5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1ea5-124">Type</span></span>   | <span data-ttu-id="d1ea5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1ea5-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d1ea5-126">ponto</span><span class="sxs-lookup"><span data-stu-id="d1ea5-126">period</span></span>    | <span data-ttu-id="d1ea5-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1ea5-127">string</span></span> | <span data-ttu-id="d1ea5-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d1ea5-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d1ea5-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d1ea5-131">data</span><span class="sxs-lookup"><span data-stu-id="d1ea5-131">date</span></span>      | <span data-ttu-id="d1ea5-132">Data</span><span class="sxs-lookup"><span data-stu-id="d1ea5-132">Date</span></span>   | <span data-ttu-id="d1ea5-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d1ea5-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d1ea5-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d1ea5-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1ea5-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1ea5-137">Request headers</span></span>

| <span data-ttu-id="d1ea5-138">Nome</span><span class="sxs-lookup"><span data-stu-id="d1ea5-138">Name</span></span>          | <span data-ttu-id="d1ea5-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1ea5-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d1ea5-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1ea5-140">Authorization</span></span> | <span data-ttu-id="d1ea5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d1ea5-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d1ea5-143">If-None-Match</span></span> | <span data-ttu-id="d1ea5-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d1ea5-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d1ea5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1ea5-146">Response</span></span>

<span data-ttu-id="d1ea5-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d1ea5-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d1ea5-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d1ea5-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d1ea5-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d1ea5-151">Report Refresh Date</span></span>
- <span data-ttu-id="d1ea5-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="d1ea5-152">User Principal Name</span></span>
- <span data-ttu-id="d1ea5-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="d1ea5-153">Is Deleted</span></span>
- <span data-ttu-id="d1ea5-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="d1ea5-154">Deleted Date</span></span>
- <span data-ttu-id="d1ea5-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="d1ea5-155">Last Activity Date</span></span>
- <span data-ttu-id="d1ea5-156">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="d1ea5-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="d1ea5-157">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="d1ea5-157">Synced File Count</span></span>
- <span data-ttu-id="d1ea5-158">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="d1ea5-158">Shared Internally File Count</span></span>
- <span data-ttu-id="d1ea5-159">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="d1ea5-159">Shared Externally File Count</span></span>
- <span data-ttu-id="d1ea5-160">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="d1ea5-160">Visited Page Count</span></span>
- <span data-ttu-id="d1ea5-161">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="d1ea5-161">Assigned Products</span></span>
- <span data-ttu-id="d1ea5-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d1ea5-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d1ea5-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1ea5-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d1ea5-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1ea5-164">Request</span></span>

<span data-ttu-id="d1ea5-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-165">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="d1ea5-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1ea5-166">Response</span></span>

<span data-ttu-id="d1ea5-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="d1ea5-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d1ea5-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
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

