---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Obtenha dados sobre as atividades do OneDrive por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 39ce2487815b1edf3cd92b9ab9b7643dac5f0a23
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591403"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="d2a0e-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d2a0e-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="d2a0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2a0e-105">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-105">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="d2a0e-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="d2a0e-106">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2a0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2a0e-107">Permissions</span></span>

<span data-ttu-id="d2a0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2a0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2a0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2a0e-110">Permission type</span></span>                        | <span data-ttu-id="d2a0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2a0e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d2a0e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2a0e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2a0e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2a0e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d2a0e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2a0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2a0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-115">Not supported.</span></span>                           |
| <span data-ttu-id="d2a0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2a0e-116">Application</span></span>                            | <span data-ttu-id="d2a0e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2a0e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d2a0e-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d2a0e-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d2a0e-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d2a0e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a0e-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d2a0e-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d2a0e-121">Function parameters</span></span>

<span data-ttu-id="d2a0e-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d2a0e-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d2a0e-123">Parameter</span></span> | <span data-ttu-id="d2a0e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2a0e-124">Type</span></span>   | <span data-ttu-id="d2a0e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a0e-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d2a0e-126">ponto</span><span class="sxs-lookup"><span data-stu-id="d2a0e-126">period</span></span>    | <span data-ttu-id="d2a0e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2a0e-127">string</span></span> | <span data-ttu-id="d2a0e-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d2a0e-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d2a0e-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d2a0e-131">data</span><span class="sxs-lookup"><span data-stu-id="d2a0e-131">date</span></span>      | <span data-ttu-id="d2a0e-132">Data</span><span class="sxs-lookup"><span data-stu-id="d2a0e-132">Date</span></span>   | <span data-ttu-id="d2a0e-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d2a0e-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d2a0e-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d2a0e-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2a0e-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a0e-137">Request headers</span></span>

| <span data-ttu-id="d2a0e-138">Nome</span><span class="sxs-lookup"><span data-stu-id="d2a0e-138">Name</span></span>          | <span data-ttu-id="d2a0e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a0e-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d2a0e-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2a0e-140">Authorization</span></span> | <span data-ttu-id="d2a0e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d2a0e-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d2a0e-143">If-None-Match</span></span> | <span data-ttu-id="d2a0e-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d2a0e-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d2a0e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a0e-146">Response</span></span>

<span data-ttu-id="d2a0e-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d2a0e-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d2a0e-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d2a0e-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d2a0e-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d2a0e-151">Report Refresh Date</span></span>
- <span data-ttu-id="d2a0e-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="d2a0e-152">User Principal Name</span></span>
- <span data-ttu-id="d2a0e-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="d2a0e-153">Is Deleted</span></span>
- <span data-ttu-id="d2a0e-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="d2a0e-154">Deleted Date</span></span>
- <span data-ttu-id="d2a0e-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="d2a0e-155">Last Activity Date</span></span>
- <span data-ttu-id="d2a0e-156">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="d2a0e-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="d2a0e-157">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="d2a0e-157">Synced File Count</span></span>
- <span data-ttu-id="d2a0e-158">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="d2a0e-158">Shared Internally File Count</span></span>
- <span data-ttu-id="d2a0e-159">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="d2a0e-159">Shared Externally File Count</span></span>
- <span data-ttu-id="d2a0e-160">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="d2a0e-160">Assigned Products</span></span>
- <span data-ttu-id="d2a0e-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d2a0e-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d2a0e-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2a0e-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d2a0e-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a0e-163">Request</span></span>

<span data-ttu-id="d2a0e-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="d2a0e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a0e-165">Response</span></span>

<span data-ttu-id="d2a0e-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="d2a0e-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d2a0e-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
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
